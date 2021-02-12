---
layout: default
title: Elysium Search Kibana
nav_order: 11
has_children: true
has_toc: false
---

# Elysium Search User Guide
## Overview
1.	Search basics
2.	Export/Import search data
3.	Optimize Search Performance
4.	Index Management
5.	Search query language
6.	Search Cheat Sheets
7.	TIME Compare
8.	Subqueries
9.	Lookup Tables


Kibana is the default visualization tool for data in Elasticsearch. It also serves as a user interface for the Open Distro for Elasticsearch [security](../security/configuration/), [alerting](../alerting/), and [Index State Management](../ism/) plugins.


## Search basics

You *can* start Kibana using `docker run` after [creating a Docker network](https://docs.docker.com/engine/reference/commandline/network_create/) and starting Elasticsearch, but the process of connecting Kibana to Elasticsearch is significantly easier with a Docker Compose file.

1. Run `docker pull amazon/opendistro-for-elasticsearch-kibana:{{site.odfe_version}}`.

1. Create a [`docker-compose.yml`](https://docs.docker.com/compose/compose-file/) file appropriate for your environment. A sample file that includes Kibana is available on the Open Distro for Elasticsearch [Docker installation page](../install/docker/#sample-docker-compose-file).

   Just like `elasticsearch.yml`, you can pass a custom `kibana.yml` to the container in the Docker Compose file.
   {: .tip }

1. Run `docker-compose up`.

   Wait for the containers to start. Then see [Get started with Kibana](#get-started-with-kibana).

1. When finished, run `docker-compose down`.


## Kibana Query Language

The Kibana Query Language (KQL) makes it easy to retrieve events from indexes or filter the results based on fields, values and operators. 
By placing cursor in the Search field, It will give suggestions to retrive the data as per Index pattern.

![kibana search sample](kql-autocomplete.png.png, "Elysium search sample")


#image 

1. If you haven't already, add the `yum` repositories specified in steps 1--2 in [RPM](../install/rpm) or the `apt` repositories in steps 2--3 of [Debian package](../install/deb).
1. `sudo yum install opendistroforelasticsearch-kibana` or `sudo apt install opendistroforelasticsearch-kibana`
1. Modify `/etc/kibana/kibana.yml` to use `elasticsearch.hosts` rather than `elasticsearch.url`.
1. `sudo systemctl start kibana.service`
1. To stop Kibana:

   ```bash
   sudo systemctl stop kibana.service
   ```


### Terms query

Terms query matches documents that contain one or more exact terms in a field.

To match documents where the response field is 200:

```bash
response:200
```

To match documents with the phrase "quick brown fox" in the message field.

```bash
message:"quick brown fox"
```
* Note: If a default field is not set, terms are matched against all fields. 
For example, a query for response:200 searches for the value 200 in the response field, but a query for just 200 searches for 200 across all fields in your index


You can also modify the values in `/etc/kibana/kibana.yml`.


### Boolean queries
KQL supports or, and, and not. By default, and has a higher precedence than or. To override the default precedence, group operators in parentheses.

To match documents where response is 200, extension is php, or both:

```bash
response:200 or extension:php
```
To match documents where response is 200 and extension is php:

```bash
response:200 and extension:php
```
To match documents where response is 200 or 404.

```bash
response:(200 or 404)
```
To match documents where response is 200 and extension is either php or css:

```bash
response:200 and (extension:php or extension:css)
```
To match documents where response is 200 and extension is php or extension is css, and response is anything:

```bash
response:200 and extension:php or extension:css
```
To match documents where response is not 200:

```bash
not response:200
```
To match documents where response is 200 but extension is not php or css.

```bash
response:200 and not (extension:php or extension:css)
```
To match multi-value fields that contain a list of terms:

```bash
tags:(success and info and security)
```

```bash
message:"quick brown fox"
```

1. Download the tarball:

   ```bash
   curl https://d3g5vo6xdbdb9a.cloudfront.net/tarball/opendistroforelasticsearch-kibana/opendistroforelasticsearch-kibana-{{site.odfe_version}}.tar.gz -o opendistroforelasticsearch-kibana-{{site.odfe_version}}.tar.gz
   ```

1. Download the checksum:

   ```bash
   curl https://d3g5vo6xdbdb9a.cloudfront.net/tarball/opendistroforelasticsearch-kibana/opendistroforelasticsearch-kibana-{{site.odfe_version}}.tar.gz.sha512 -o opendistroforelasticsearch-kibana-{{site.odfe_version}}.tar.gz.sha512
   ```

1. Verify the tarball against the checksum:

   ```bash
   shasum -a 512 -c opendistroforelasticsearch-kibana-{{site.odfe_version}}.tar.gz.sha512
   ```

   On CentOS, you might not have `shasum`. Install this package:

   ```bash
   sudo yum install perl-Digest-SHA
   ```

1. Extract the TAR file to a directory and change to that directory:

   ```bash
   tar -zxf opendistroforelasticsearch-kibana-{{site.odfe_version}}.tar.gz
   cd opendistroforelasticsearch-kibana
   ```

1. If desired, modify `config/kibana.yml`.

1. Run Kibana:

   ```bash
   ./bin/kibana
   ```


### Range queries

KQL supports >, >=, <, and ⇐ on numeric and date types.

```bash
account_number >= 100 and items_sold <= 200
```

1. Download the ZIP.

1. Extract [the ZIP file](https://d3g5vo6xdbdb9a.cloudfront.net/downloads/odfe-windows/ode-windows-zip/odfe-{{site.odfe_version}}-kibana.zip) to a directory and open that directory at the command prompt.

1. If desired, modify `config/kibana.yml`.

1. Run Kibana:

   ```
   .\bin\kibana.bat
   ```


### Date range queries

Typically, Kibana’s time filter is sufficient for setting a time range, but in some cases you might need to search on dates. Include the date range in quotes.

	```
	@timestamp < "2021-01-02T21:55:59"
	```
	```
	@timestamp < "2021-01"
	```
	```
	@timestamp < "2021
	```


1. Download [the EXE file](https://d3g5vo6xdbdb9a.cloudfront.net/downloads/odfe-windows/odfe-executables/Open_Distro_For_Elasticsearch_Kibana_{{site.odfe_version}}.exe), run it, and click through the steps.

1. Open the command prompt.

1. Navigate to the Kibana install directory.

1. If desired, modify `config/kibana.yml`.

1. Run Kibana:

   ```
   .\bin\kibana.bat
   ```


### Exist queries
An exist query matches documents that contain a value for a field, in this case, response:

```
response:*
```
1. After starting Kibana, you can access it at port 5601. For example, http://localhost:5601.
1. Log in with the default username `admin` and password `admin`.
1. Choose **Try our sample data** and add the sample flight data.
1. Choose **Discover** and search for a few flights.
1. Choose **Dashboard**, **[Flights] Global Flight Dashboard**, and wait for the dashboard to load.

### Wildcard queries

To match documents where machine.os starts with win, such as "windows 7" and "windows 10":

```
machine.os:win*
```
To match multiple fields:

```
machine.os*:windows 10
```
The query checks machine.os and machine.os.keyword for the term windows 10.

### Nested field queries
