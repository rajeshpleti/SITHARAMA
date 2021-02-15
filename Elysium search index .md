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
5.	Search query language (KQL)
6.	Search Cheat Sheets
7.	TIME Compare
8.	Subqueries
9.	Lookup Tables


Kibana is the default visualization tool for data in Elasticsearch. It also serves as a user interface for Elysium Security , Alerting  and Index State Management plugins.


## Search basics

To search the indices that match the current index pattern, enter your search criteria in the query bar. By default, you’ll use Kibana’s standard query language (KQL), which features autocomplete and a simple, easy-to-use syntax.

### About Search Basics
Elysium search syntax is based on "pipeline" concept and it uses logical and familiar operators letting you to create ad hoc queries quickly.
### Built-in Metadata
Metadata tags are attached to your log messages at ingest, which is very useful when you're searching log data.
### Chart Search Results
In the Aggregates tab, in addition to the standard table view, you can view search results as a chart, such as a bar or column chart.
### Comments in Search Queries
You can add comments to a search query, or even comment out lines of your search query using comment formatting.
### Export Search Results
Up to 100,000 rows can be exported  as a CSV (comma-separated values) text file.
### Pause or Cancel a Search
When a search is in progress, the options to Cancel or Pause the search appear.
### Quick Search for Collectors and Sources
You can quickly start a search for a Collector, Source, or Source Category from the Manage Collection page.
### Reference a Field with Special Characters
Solution to reference a field name that contains a special character
### Save a Search
Whether you are running ad hoc searches during a forensic investigation or running standard searches for health checks, you can save any search to run later.
### Search Autocomplete
On the Search page, as you begin typing to enter a query in the search text box, the search autocomplete drop-down dialog opens to offer suggestions to make query writing easier.
### Search Large Messages
When collecting log messages or event logs that are larger than 64KB in size, Elysium slices the messages into a stream of smaller message chunks.
 ### Search Surrounding Messages
Surrounding messages allow you to investigate events surrounding a message.
### Share a Link to a Search
Copy and paste the a link to share a search via email or IM.
### Time Range Expressions
When you are building a search query, you have the option to add a time range expression in the time range field.
### View Search Results for JSON Logs
If your search results contain JSON logs, you can expand or collapse the view on the Messages tab to show or hide the JSON format and structure.



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


![Demo CountPages alpha](https://www.youtube.com/watch?v=ek1j272iAmc)

[![Demo CountPages alpha](https://share.gifyoutube.com/KzB6Gb.gif)](https://www.youtube.com/watch?v=ek1j272iAmc)

![Search](kql-autocomplete.png)
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


## Optimize Search Performance

Search optimization tools speed the search process, delivering query results in less time and improving productivity for forensic analysis and log management.

Search speed generally depends on the amount of data and the type of query run against the data. Search optimization tools segment the data and queue it up for quick results.

An index, or proper subset of the data, is central to search optimization. When you run a search against an index, search results are returned more quickly and efficiently because the search is run against a smaller data set.

Elysium supports index-based and field-based methods for search optimization.

## Index-based methods

Partitions route unstructured data into an index. See how to Optimize Your Search with Partitions.

Scheduled Views pre-aggregate data and then index it.
## Metadata methods

With metadata tags assigned to your logs you can reference them in the scope (keyword search expression) of queries to drastically increase search performance.

Metadata is typically from your system or environment, and adds context about what or where the data came from and any associated services or apps. Logs and metrics use metadata that can be customized to anything you need.

Log metadata - In addition to having more data to reference in query operations, this allows you to define a more specific scope of data in search expressions, improving search performance, and allows more specific search filters in Roles and routing expressions in Partitions.

Metric metadata - Elysium provides a number of features you can use to enrich the metrics you collect with metadata. Metric metadata provides considerable benefits when you query your metrics: you can scope your metric queries to return only the metrics of interest. 
