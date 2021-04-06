


# Elysium Analytics and AI Documentation

## Contents 

## 1. [Key Features Of Elysium Analytics](#KeyFeatures)
	1. Insider Threat Detection 
	2. Privileged Account Usage 
	3. DNS Tunneling
	4. VPN Monitoring
	5. Unusual File Access
	6. Data Exfiltration
	7. Bot Attack 
	8. Unusual File Downloads
	9. Leverage data science platforms (Advanced AI/ML Techniques)
	10. Phishing Attack
	11. New IP Addresses
	12. Build your own Analytical dashboards
## 2. [Quick Start](#quickstart)
	1. After filling the client form
	2. Setup Client access using UI
	3. Setup cloud access
	4. Setup Installation, Services offering
	5. 10 days trail run if any
	6. Request a Demo

## 3. [APP’S Integration](#APPS)
	
1. [360 view](#360view)
1. [Alerts](#alerts)
1. [Endpoint](#endpoint)
1. [ITD (Inside Threat Detection)](#ITD)
1. [Identity Management](#IM)
1. [Operational Dashboards](#operationaldashboard)
1. [Search](#search)
1. [Statistical Data](#statisticaldata)
1. [Security Posture](#securityposture)
1. [Behavior Analytics UEBA](#UEBA)
1. [Snowflake analytics](#snowflakeanalytics)
1. [Source analytics](#sourceanalytics)
1. [SOC Dashboard](#socdashborad)
1. [NIST,HIPAA,SOX](#NIST)

## 4. Inside Threat Detection 
1. [Filters](#filters)
1. [Behaviours of Risky User and Entity(Day wise and aggregation)](#behaviourofrisky)
1. [Anomaly count user/Entity source](#anomalycount)
1. [Threat User’s and Entity](#threatuserentity)
1. [360 User view](#360userviewmain)
1. [360 IP View](#360ipwmain)
1. [Risk score trend analysis for User/ Entity](#riskscoretrendanalysis)
1. [Daily Risky Behavior – Zscores](#dailyriskyzscores)
1. [MITRE-ATTACK and Alerts](#MITREattack)
1. [Event level Risk Trend](#eventlevelrisktrend)
1. [Event List](#eventlist)
 
	 

## 5. Profile (User/Entity anomaly Scores) or UEBA(User and Entity Behavior Analytics)
1. [Endpoint Indicators of Compromise](#endpoint1)
2. [Privileged Account Usage](#previlegedaccount)
3. [High Volume File Access](#highvolumeaccess)
4. [Bandwidth Usage by size and count](#bandwidthsizecount)
5. [VPN Connections](#vpnconnections)
6. [File Downloads](#filedownloads)
7. [Bot Attack](#botattack)
8. [Unusual Domain](#unusualdomain)


## 6. [Build your own Analytical Dashboards](#buildanalytics)
### 6.1. [looker creation of dashboards](#lookerdashboard)

1. [Creating A New Dashboard in Elysium Analytics](#newdashboard)
1. [Adding new tiles to dashboard](#newtiles)
1. [Looker Explore window to discover new insights](#explore) 
1. [Select the fields and  filters for your query tile’s](fieldsandfilters)
1. [Configure your visualization options](#visualizations)
1. [Adding Dashboard Filters a User Can Change](#usercanchange)
1. [Copy Of Existing Dashboard and Editing the dashboard](#copy1)
1. [Users and Roles of access of dashboards](#userroles)
1. [Dashboards Available in Elysium Analytics](#availabledashboards)

### 6.2. [Elysium Kibana Data Visualizations](#kibanaviz1) 

### 6.3. [Build Kiabana Dashboards](#mainkibanadashboard)  
1. [Visualize your data with dashboards](#yourdashboard)
1. [Open the dashboard](#opendashboard)
1. [Create panels](#createpanels)
1. [clone panels](#clonepanels)
1. [Explore the underlying documents](#exploredocuments)
1. [Download panel data as CSV](#downloadpanel)
1. [Share the dashboard](#sharedashboard)
1. [Export the dashboard](#exportdashboard)


## 7. Data Collection and Ingestion 

1. [Collect your data/Shippers](#shippers)
2. [Connectors and plugins](#connectyourdata)
3. [Parsing data](#parsedata)
4. [Enrich data](#enrichdata)
5. [Loading data](#loaddata)
6. [Add Threat intelligence to your data](#addthreat)
7. [Cloud Apps](#cloudapps)
8. [Data Investigation Dashboards](#investigationdashboard)
9. [Data Ingestion tracking](#ingestiontracking)
10. [Logstash Network Traffic Dashboards](#LogstashNetwork)

## 8. Alerts
	1. Alerts monitor
	2. Scheduled searches
	3. Alert rules
	4. Alert creation
	5. Alert action
	6. Alert Notification
	7. Alert Dashboards
	8. Drill Down Alerts

## 9. Search

1.Search basics
1.Search query language (KQL)
1.KQL Introduction
1.Search multiple fields
1.Grouped together
1.Terms query
1.Boolean queries
1.Range queries
1.Date range queries
1.Exist queries
1.Wildcard queries
1.Nested field queries (Subqueries)
1.Optimize Search Performance
1.General Search Examples
1.Supported Logs
1.Standard Fields (ODM)
1.Backend snowflake integration, SQL Opendistro query support for Elysium kibana search
1.Save query, search
1.Index Management
1.Create Filters and search 

## 8. Manage and Monitoring
1. Ingestion and Volumes
2. Users and Roles
3. Connections and Integration
4. Data Forwarding

## 9. SIEM (Security Information and Event Management )
1. Hosts
2. Network
3. Endpoint Activity
4. Authentication logs
5. DNS Traffic
6. NetFlow

## 10. Role-Based Access Control
1. Admin Role 
2. Analyst Role 
3. Developer Role 
4. Manger Role 
5. Team Lead Role 
6. Dashboard Access control

## 11. Cloud Integration
1. AWS
2. GCP
3. Azure
## 12. Support Help
1. Community help github
2. Product support 
3. Virtual assistance chatbot




## Details of contents 


# 1. Key features Of Elysium Analytics <span id="KeyFeatures"><span>
	
	
* Elysium Analytics is a machine learning based log analysis solution for security minded mid-sized to large enterprises, challenged by the volume of security log data today both from an infrastructure as well as an analytics and detection perspective.

* We have simplified onboarding of data, provide a scalable data lake analytics platform, and search on a pay-as-you-go basis . 
* Since we are built on top of Snowflake, our SaaS solution is truly a cloud scale security analytics platform that removes the barriers from ingesting, contextualizing, 	searching, analyzing, and storing log data with a cost effective and low risk service. 
*  Unlike the other log analysis vendors in this market, our SaaS offering is licensed on a usage basis lowering cost and reduces financial risk.  You pay a low price for storage, and compute is billed by the minute of usage.  
* Additionally, we have an open platform with no vendor lock-in, customizable analytics models, as well as APIs for end user development of analytics models. 


* Elysium Analytics provides a single pane of glass through an SOC analyst identifies, observes  aggregated views of all activity of users and entities across an enterprise.
* This is achieved through the use of profilers, perform data sketches across time intervals on security metrics to baseline, behaviours of users and entities, MITRE ATT&CK vectors. 

* To unify the underlying data schema, Elysium Analytics has created an advanced “layered” schema architecture that supports different log vendors  “views” into the same ODM schema. 
* Elysium is committed to providing open security framework deployments with add-ons that enable our customers to utilize analytics created by security framework.

**1. Insider Threat Detection:**

Insider Threat Detection Show users, Entity's deviating from normal behavior and detect statistical anomalies and outliers with unsupervised learning clustering across numerous features, outliers and indicators of compromise threshold values of risk factors.
Elysium ITD detects early indicators of insider threats Users/Entity's, Behaviours,  prevent insider threats,alerting, mitigate their consequences of actions.

**2. Privileged Account Usage:**

Identify privileged users, services, and shared accounts and then monitor them for abnormal usage associated with insider and external attacks.

**3. DNS Tunneling:**

Detect DNS tunneling attacks used for malicious file transfers, payload downloads, or remote access.

**4. VPN Monitoring:**

Profile geo-location of users & endpoints and compute the number of simultaneous VPN connections during any minute of any day to detect unauthorized access.

**5. Unusual File Access:**

Identify excessive and abnormal file activity on endpoints and detect individuals, or malware controlled by attackers, attempting to search for and steal valuable digital assets.

**6. Data Exfiltration:**

Detect unauthorized transfer of data from a user's computer or servers carried out by someone manually or automatically by malware on the network.

**7. Bot Attack:**

Detect bot traffic and attacks in real-time by monitoring high velocity connections and port scans across devices within the corporate network.

**8. Unusual File Downloads:**

Protect your network and  users from malicious content and binaries by detecting downloads from low prevalence and suspicious sites and domains.

**9. Leverage data science platforms (Advanced AI/ML Techniques):**

Build your own ML models on Databricks or other preferred data science platforms to  detect new evolving threats.

![ml](ml.png)

**10. Phishing Attack:**

Profile email use patterns and detect unusual and potentially high risk email messages from low prevalence and suspicious domains.

**11. New IP Addresses:**

Protect your network and users from malware downloads, drive-by attacks, and phishing attacks through profiling of new IPs and detection of connections to low prevalence IPs.

**12. Build your own Analytical dashboards:**

Build your own analytics dashboards with Looker or connect to 3rd party applications through our API.


# 3. APP’S Integration  <span id="APPS"><span>
	
Elysium APP'S Integration 

![apps](appstoremain.PNG)

### 1. 360 view <span id="360view"><span>
	
Elysium offers to show all the information of a user or an entity for Last 30 Days.
Shows login patterns (successful & failed logins) for the last 7 and 30 days for the user/entity in context
Shows all machines access for the last 7 days and 30 days by users and entity’s
Amount of data pushed to web versus his community
Access to any suspicious or dark sites.
Show escalated privileges by user/entity

### 2.	Alerts <span id="alerts"><span>
<p style='text-align: justify;'> 
Elysium alerts Monitors continuously query your data to monitor and send notifications when specific events occur.
thresholds, critical, warning, and missing data and also gives aggregation based results.

Elysium offers a set of correlation rules and behavioral analytics to alert on specific sequence of events or pattern using machine learning and statistical analysis. 
The alerting feature notifies you when data from one or conditions are met. 
For example, you might want to receive an email if your application logs more than five HTTP 503 errors in one hour, or you might want to page a developer if no new records have been processed in the past 20 minutes.
</p>	
	
### 3.	Endpoint <span id="endpoint"><span>
Endpoint Dashboard analysis provides traffic and attacks in real-time by monitoring high velocity connections and port scans across devices within the corporate network.
It supports Profile geo-location of users & endpoints and compute the number of simultaneous VPN connections during any minute of any day to detect unauthorized access
1. VPN Monitoring
1. Unusual File Access
1. Data Exfiltration
1. Bot Attack 
### 4.	ITD (Inside Threat Detection) <span id="ITD"><span>
<p style='text-align: justify;'> 	
Inside Threat Detection identifies abnormal behaviors of user/entity using unsupervised learning algorithms and provides statistical anomalies scores ,outliers and indicators of compromise threshold values of risk factors.

It provides simple dashboards easily understood by users. 
It has scoring:  0 to 60% normal, 60 to 90 as unsafe behavior, and 90% or higher as insider threat. 
By using risk-based Scoring, which performs data sketches across time intervals on security metrics baselining the behaviors of all users and entities,
we gain full visibility into any anomalous and suspicious behavior through risk-based scoring of the security data.
</p>

###  5.	Identity Management <span id="IM"><span>
VPN Session dashboard explain about:
1. The name of user connecting and disconnecting,
1. The start and end time of the VPN or administrator sessions,
1. The outside global address from where the user and host connect
1. The inside local address assigned to the user's session.

### 6.	Operational Dashboards <span id="operationaldashboard"><span>
	
We combine all your on-prem IT logs, enterprise network logs, cloud logs and network traffic data into one scalable data lake and combine your in-cloud and on-prem data silos into one scalable Snowflake data lake. 
We map, parse, and store your data in Elysium Analytics Open Data Model for full context and fast analytics. 
We have an Operational folder in our App where you can find Data Investigation and Data Collection Reports.
	
### 7.	Search <span id="search"><span>
Kibana is the default visualization tool for data in Elasticsearch. It also supports querying integration interface with snowflake, SQL, Kibana Query Language (KQL).
The Kibana Query Language (KQL) makes it easy to retrieve events from indexes or filter the results based on fields, values and operators and features autocomplete,simple, easy-to-use syntax. 
By placing cursor in the Search field, It will give suggestions to retrive the data as per Index pattern.
Elysium search syntax is based on "pipeline" concept and it uses logical and familiar operators letting you to create ad hoc queries quickly.

### 8.	Statistical Data <span id="statisticaldata"><span>
A Statistical dashboard is an information management tool that visually tracks, analyzes and displays metrics and key data points to monitor the user information.
	
### 9.	Security Posture <span id="securityposture"><span>
The Security Posture dashboard is designed to provide high-level insight into the notable events across all domains of your deployment, suitable for display in a Security Operations Center (SOC). 
This dashboard shows all events from the past 24 hours, along with the trends over the past 24 hours, and provides real-time event information and updates.  
This dashboard is fully customizable and gives a bird’s eye view into all notable events across all domains of security. 
	
### 10.	Behavior Analytics UEBA <span id="UEBA"><span>
UEBA utilizes machine learning and other advanced analytics to detect threats and simplify the work of technical professionals focused on security. 
Furthermore it offers a signatureless approach for detecting emerging threats with statistical analysis and machine learning.  
Specifically Elysium offers canned UEBA reports that map specific techniques and tactics from MITRE ATT@CK vectors, encoding them into behavior profiles that detect unusual behaviors.

### 11.	Snowflake analytics <span id="snowflakeanalytics"><span>
Snowflake audit dashboards can be provided using Advanced Machine learning techniques to provide descriptive statistics of user usage aacount details, identifying abnormal behaviour, anomoly scoring, alerting. 
1. Snowflake audit logs
1. Snowflake login history
1. Alert scoring
1. Timeseries Scroing 
1. Anomaly scores 
	
### 12.	Source analytics <span id="sourceanalytics"><span>
	
Source Analytics dashboard mainly focuses on windows auditing, security, Network traffic data with what type of events occurred in a day for each host and user.
	
### 13.	SOC Dashboard <span id="socdashborad"><span>
	
Security operations center (SOC) managers can view overall efficiency metrics and measure the individual performance of the SOC team members in the organization. 
This dashboard explains about all key information of the organization.

### 14.	NIST,HIPAA,SOX <span id="NIST"><span>
	
### NIST (National Institute of Standards and Technology)
Companies that provide products and services to the government have to follow some policies set by the National Institute of Standards and Technology (NIST). NIST has two common mandates (NIST 800-53 AND NIST 800-171 which companies have to follow.
These are the reports Offered by Elysium.
1. Resource Monitoring
1. Remote Access
1. Trust Relationships 
1. Continuous Monitoring
1. User Access and Least Privileges
1. File Integrity Monitoring
1. Change Control  
1. Boundary Defenses
1. Login and Logoff Monitoring
1. Investigation Reports
1. System Events
1. Email reports
1. Watchguard DHCP Reports
1. Watchguard Proxy Reports 

### HIPAA
HIPAA Deals with health care organizations where data is sensitive and critical. So Elysium offers to collect and analyze the logs with meaningful information in the form of reports.These are the reports Offered by Elysium.
1. Logon and Logoff Monitoring
1. Account Logon
1. System Events
1. Object Access

### SOX IT Compliance

SOX Regulations that mandate accuracy, integrity and security of the company or an organization. 
1. It processes log data which is tedious. To make it easy Elysium offers predefined reports.These are the reports Offered by Elysium.
1. User Logon and Logoff
1. Logon Failure
1. User Access
1. Successful or Unsuccessful Validation & User group changes
1. Continuous Monitoring











## 4. Inside Threat Detection   <span id="ITD"><span>

Elysium Analytics provides a unique AI-driven security analytics platform that comes with a wide array of advanced ML-based security outcomes and behavioural models to help organizations detect and respond to advanced cyber-attacks. 
1. It Reduces costs of an insider attack 
2. Early detection of insider threat
3. Fast and efficient response to an insider attack. 
4. Alerting and Notfications 
	
Inside Threat Detection identifies abnormal behaviors of user/entity using unsupervised learning algorithms and provides statistical anomalies scores ,outliers and indicators of compromise threshold values of risk factors. 
	
An Elysium insider threat program is  a efficient core part of modern cybersecurity strategy. Elysium ITD controls in place to detect, deter, and respond to insider attacks and inadvertent data leaks is a necessity for any organization that strives to protect its sensitive data. It’s also required by many IT regulations, standards, and laws: NISPOM, NIST, HIPAA, PCI DSS, and others.

Elysium ITD detect insider threats based on 
1. Monitor User/Entity activity
2. Manage User/Entity access to sensitive resources
3. Analyze User/Entity behavior

Elysium Perform a risk assessment based on 

1. Define threat sources 
2. Discover cybersecurity vulnerabilities
3. Create list of high risk employess and high value assests 
4. Estimate the liklihood insider threat based on timeseries of events
5. Determine and assess risk scores
6. Alerting and Notfication to make corresponding actions.

### Overview of the ITD tiles in the Dashboard
### 1.	Filters  <span id="filters"><span>

Filters:  User can Change the  Date filter,User filter and RUN the Dashboard
 

Date fillter supports is in the past, is on the day, is in the range, is in the year, is any time, is null, is not null etc.
User filter supports is equal to, contains, starts with, ends with, is not null, is null matches user attribute etc.

![capsutre](Capture.PNG)

![capsutre](Capture1.PNG)
	
### 2. Behaviours of Risky User and Entity(Day wise and aggregation)  <span id="behaviourofrisky"><span>

User/Entity Count with High Risk Scores
It shows the Score of high risky events
	
![riskbehaviour](behaviour.PNG)
	
	
### 3.	Anomaly count user/Entity source <span id="anomalycount"><span>
Anomalous User/Entity by Source
It shows the count of high anomaly score  and source types


![anamolycount](anamolycount.PNG)
	
	
### 4.	Threat User’s and Entity <span id="threatuserentity"><span>

Threat Users
It shows data for max score for all Users in Elysium Analytics in the last 15 days
Threat Entities
It shows data for max score for all Entities in Elysium Analytics in the last 15 days


![threatusersandentity](riskscoreofuserentity.PNG)
![top10users](top10users.PNG)
	
	
### 5.	360 User view <span id="360userviewmain"><span>
	
![user3601](360userview.PNG)


Overview of the Tiles in Dashboard
1. Active Directory shows the details of AD User.
1. Risk Score shows the Average of the Risk Score in a weeks time for Source Type -  ML-AGGREGATE
1. Alerts Count shows the count of alerts in a week
1. Number of Assets shows the count of IPs accessed in a week.
1. Aggregates show the Count of Aggregates
1. Risk Score Trend Analysis shows the sum of Risk score per day for 2 weeks for source Type - ML
1. High Risk Analysis shows the sum of events based Anomaly Score 
1. Daily Risky Behavior - Zscores shows the different  Scores for source type - ML in last 15 days
1. MITRE - ATTACK shows details about the Mitre attack for User in past 2 weeks
1. Alerts shows the Count of Alerts per Type.
1. Event Level Risk Trend shows the sum of User Anomaly score for type other than ML in the past 15 days
1. Event List shows the details of events like description, IP, Anomaly score etc.
1. If you click on Src User name or Src IP , you will get different options to drill down and see the details.
	
### 6. 360 IP View  <span id="360ipmain"><span>
	
![userIP](user3609.PNG)		
	
Filter: User can change the filter and run the dashboard 

Overview of the Tiles in Dashboard

1. Risk Score Trend Analysis for Entity shows the sum of risk score of entity / IP for Src Type ML on a day  in the past 15 days.
1. Anomaly Score Trend Analysis for Entity shows the sum of Anomaly score of entity / IP  for Scr Type ML on a day to the past 15 days.
1. High Risk Events shows the total count per Source Type - Security Auditing , Network traffic etc other than type ML with Anomaly score >=85 in past 15 days
1. Profile Z Score shows the details 
1. Time Series shows Sum of If Dwnld Ts and If Dwnld Val per day for last 15 days for ML
1. Alerts shows Count of Alerts by Alert name
1. Event Level Risk Trend shows the sum of User Anomaly score for type other than ML in the past 15 days
1. Event List gives the details about the Event with Entity anomaly score >=85 and Dst name in the past 15 days


### 7.	Risk score trend analysis for User/ Entity <span id="riskscoretrendanalysis"><span>
	
Anomaly Score Trend Analysis for Entity shows the sum of Anomaly score of entity / IP  for Scr Type ML on a day to the past 15 days.	
	
![riskscore](user3608.PNG)	
	
![riskscoreenity](user36010.PNG)
	
### 8.	Daily Risky Behavior – Zscores  <span id="dailyriskyzscores"><span>
Z_score value gives the amount of abnormal deviation of an object (user/enity) from the population by considering its previous behaviour over time series along with other objest behaviour .
Daily Risky Behavior - Zscores shows the different  Scores for source type based machine learning techiques in last 15 days.
Ex: Logins Zscore, Failedlogins Zscore,  If Upld Zscore, If Dwnld Zscore, Fileactivity Zscore, Email Count Zscore



![user3603](user3603.PNG)	
	
### 9.	MITRE-ATTACK and Alerts  <span id="MITREattack"><span>
MITRE ATT&CK is a framework describing tactics and techniques for how adversaries attack computers and networks.  "ATT&CK" is an abbreviation of "Adversary Tactics and Techniques and Common Knowledge". 
The Enterprise ATT&CK matrix is Elysium's priority interest and focuses primarily on hosts using Microsoft Windows and Microsoft Windows Server operating systems. The Enterprise matrix include techniques applicable to Linux and MacOS hosts also.

Alerts shows Count of Alerts by Alert name
Filter by Alert name will open another dashboard and see the details about the particular Alert
It shows data for max of Total Alert Count,Max of Alert Score,Max of Anomaly Score,Max of Risk Score.They are represented in different colored Bars.

![user3604](user3604.PNG)	
![alertssoc](alerts.PNG)
	
### 10.	Event level Risk Trend  <span id="eventlevelrisktrend"><span>
Event Level Risk Trend shows the sum of User Anomaly score for type other than ML in the past 15 days	
![eventlevelrisktrend](user3607.PNG)	
	
### 11.	Event List  <span id="eventlist"><span>
Event List shows the details of events like event Timestamp, src username, description, IP, Anomaly score, in bytes, out bytes, event id,  etc	
	
![eventlist](user3605.PNG)	
	
	
## 5. Profile (User/Entity anomaly Scores) or UEBA(User and Entity Behavior Analytics) <span id="UEBA"><span>
	
	
UEBA utilizes Machine Learning and Advanced Artificial Intelligence (AI) analytics to detect threats and simplify the work of technical professionals focused on security. 

Furthermore it offers a signature less approach for detecting emerging threats with statistical analysis, AI and machine learning approaches.   

Elysium UEBA (User and Entity Behavior Analytics) provides solutions for profile users, their peer groups and other entities, employ advanced analytics to detect anomalous transactions,  behaviors and  User/Entity endpoints.

Algorithm,anomaly score range,anomaly outliers threshold, Count of Users,Information,Outliers,Details are common  in all the UEBA’s.They vary with respective UEBA view used and All the tiles in dashboards changes according to the Parameters of the UEBA, Those parameters  appear in the Information tile.

![overviewUEBA](overviewUEBA.PNG)

## **Overview of all the UEBA’s**

* Bandwidth Usage by Count shows the Average of Downloaded Bytes,Average of Uploaded Bytes Information.
* Bandwidth Usage by Size shows the Average of Sent Bytes,Received Bytes information.
* EndPoint Indicators of Compromise shows the Average of Sent Bytes,Average of End Point  Remote count Information.
* Privileged Account Usage shows average of bandwidth and average of privileged count information.
* High volume File Access shows average of file access and average of file volume count Information
* VPN CONNECTIONS shows  Avg Distance of Geo-locations between Sessions and  Total no.of sessions information
* File Downloads shows Average of Destination count and Average of Download  Count information.
* Bot attack shows average of source count,average of destination count information.
* Unusual Domain shows the average of uploaded bytes and average of Distinct Domain count information




## User session Tracking information
1. User session Tracking Dashboard has on information related to these below:
1. Bandwidth usage
1. File downloads/uploads
1. Top visited sites
1. Top block sites
1. Cloud Applications
1. Mobile Traffic by Device Type
1. Mobile Traffic by Location
1. Locations
1. Social Networking Applications
1. Streaming Media Application
1. VPN session activity
1. Email Counts & Size.

## **Overview of the Tiles in User session tracking Dashboard**

1.Total Web Traffic Count, Bandwidth (Upload and Download Bytes) and Location of Users for Event Ids 
1. Windows Session Tracking shows the details like Session Start time, End Time, IPs, Description, Duration of the session etc for Windows
1. WatchGuard Session Tracking shows the details like Session Start time, End Time, status, user etc for WatchGuard
1. Top visited Sites shows the details of Domain, Web category, count etc a particular user has accessed in  WGTraffic
1. Overall traffic give you the details like user, IP, Bandwidth etc 
1. Cloud Application will gives you the details such as User name, session start time, Web category etc
1. Top Blocked Sites gives you the details  of the blocked sites a user has access.
1. Streaming Media Application shows the details of category Streaming Media, Entertainment, Internet Telephony etc
1. Social Networking Application shows the details of users who are using Social media like Facebook, Twitter, YouTube, LinkedIn etc
1. Email Count & Size  shows the details of emails.
1. Blocked Transactions gives you details like user name, Domain etc  for web categories like Games, Potentially unwanted software etc or with a message like 'ProxyDeny: 1. HTTP Request categories','ProxyDrop: HTTPS Request categories'


## **Overview of the Tiles in UEBA  Dashboard**


### 1.	Endpoint Indicators of Compromise <span id="endpoint1"><span>
Mobile/Laptop/Desktop Device Malware Scan 
The following Dashboard is the data on all events containing "Symantec".
The data on severity level, user's log/event channel and source information were all compiled in this dashboard


* End points on the Network and Anti malware Scan Status shows the Symantec Endpoint protection client and active directory hostname ,description of the status in the past 7 days
* Fraction of Hosts in various states shows the status ,count of the union of symantec endpoint and active directory Host.
* Summary of Malware Risk Activities shows the Malware,Action and its description,Hostname .
* HostName viruses shows the malware name,host name, count of symantec endpoint protection Client  in the past 7 days.
* Antimalware Software Events shows the names of host,malware,Activities and Counts of file,risk and events in the Symantec End point in the past 7 days.


![endpoint](uebaendpoint.PNG)	
	
### 2.	Privileged Account Usage <span id="previlegedaccount"><span>
Details View shows the details like source name,source ip ,source geo city,count in the ITD 360 view .
Ip Geo Map shows the locations of the user and the count.
It redirects to the dashboard with Details View,IP GEO MAP changed.These two tiles are filtered  with new user value

![privilegedac1](previllagedac1.PNG)	
![privilegedac2](previllaed2.PNG)

### 3.	High Volume File Access  <span id="highvolumeaccess"><span>
High volume File Access shows average of file access and average of file volume count Information	
![highvolumes](highvolumes.PNG)	
	
### 4.	Bandwidth Usage by size and count  <span id="bandwidthsizecount"><span>

* Bandwidth Usage by Count shows the Average of Downloaded Bytes,Average of Uploaded Bytes Information.
* Bandwidth Usage by Size shows the Average of Sent Bytes,Received Bytes information.

![Bandwidthsize](bandwidthsize.PNG)	
![Bandwidthcount](bandwidthbycount.PNG)		
	
### 5.	VPN Connections   <span id="vpnconnections"><span>

 1. WatchGuard Session Details shows the information Session,User , source  and host in the past 30 days
 2.  Count of WatchGuard Sessions by Device  Shows the Start time of the Session and count of 
      the  sessions per hostname in the past 30 days.Click on the graph Drill into appears.Click 
      on any of the sessions start Date time Hour,Minute or Time Details appear.
3.  Session status shows the status ,count of the Sessions.
4.  Watchguard Session Types shows the type and Count of the Sessions.
5.  More Watchguard Session of the User shows the user name and count of the Sessions.
6.  Locations of the VPN Sessions shows the count of sessions in the locations
7.  Failed Login  shows the Event  occurred information like user name,
    source information,hostname and the notification information in the message in the 
     past 30 days.

![vpnconnections](vpnconnections.PNG)			
	
### 6.	File Downloads  <span id="filedownloads"><span>
* File Downloads shows Average of Destination count and Average of Download  Count information.	
![filedownloads](filedownloads.PNG)	
	
### 7.	Bot Attack  <span id="botattack"><span>
*  Bot attack shows average of source count,average of destination count information.
![botattack](botattacks.PNG)	
		
	
### 8.	Unusual Domain  <span id="unusualdomain"><span>

* Unusual Domain shows the average of uploaded bytes and average of Distinct Domain count information	
![unusual](unusual.PNG)	




## 6. Build your own Analytical dashboards <span id="buildanalytics"><span>

* Elysium  visualize your data into dashboards, combining tables, charts in useful and interesting layouts, aggregations to the axes, filtering data interactively based on logical conditions, choose modes and colors of charts, and place legends and labels.
* This modules explains how to use the Elysium Analytics user interface to create a new dashboard and populate it with visualizations
* A dashboard is essentially a collection of visualizations of tiles, displayed all in one page. It allows to add filters to make the dashboard interactive and rearrange its tiles and shares visualization dashboard to team memebers based on access roles.

## 6.1 looker creation dashboards  <span id="lookerdashboard"><span>

### 1. Creating A New Dashboard in Elysium Analytics <span id="newdashboard"><span>

To create a blank dashboard:

 	1. Click New Dashboard.
	2. Name the Dashboard.
	3. Click Create Dashboard

![newdashboard2](newdashboard2.PNG)

another option is go to personal folder of Looker after entering the credentials https://elysiumanalyticsstaging.cloud.looker.com/ then click on New dashboard option. 
![personalfolder](newdashboard1.PNG)

### 2. Adding new tiles to dashboard <span id="newtiles"><span>
After creating emptydashboard, editdashboard,  add new tiles to dashboard 

![addtiles](addtile.PNG)

### 3. Looker Explore window to discover new insights  <span id="explore"><span>

Adding New Tile opens a menu of Explores. Choose an Explore view to build dashboard based on different types supported dashboards views already existed in elysium analytics.Explore AWS,Azure,graph Test, Insider trading, IOT, Insider threat detection, Marketing, ODM, Redsky, snowfalke Usage,SQL master, sstech, stock details,  system activity, stubhub, Timelines etc.

![explore](explore1.PNG)

![explore2](explore2.PNG)

It contains three modules
1. Filters
2. Visualization
3. Data

![sample](snowflakestorage.PNG)

### 4. Select the fields and  filters for your query tile’s <span id="fieldsandfilters"><span>

First select data fileter, then choose relevant fields and filters for query tiles to visually analyze the insights of data

![filters](filterfields.PNG)

### 5. Configure your visualization options <span id="visualizations"><span>
	
configuration options allows users to change the visualization based on various parameters

1. Create and run your query.
1. Click the Visualization tab to start configuring your visualization options.
1. Select the type of visualization that best displays your data. For more options, click … to the right of the displayed visualization options.
1. Click Edit to configure the visualization option settings, such as naming and arranging chart axes, choosing the position and type of each data series, or 		     modifying the chart color palette.
1. Once you have set up your query, click Run.
1. Click Save to save the query as a tile on your dashboard.
1. Same way we can add  multiple tiles to the dashboard


![config1](config1.PNG)

![config2](config2.PNG)

### 6. Adding Dashboard Filters a User Can Change <span id="usercanchange"><span>

![parameters](addfilterdashboards.PNG)

1. Click on Filter to create a new filter. Elysium lists the new filter on the left hand side of the filters pop-up. You can drag and drop the filters to control the       order in which they appear on the dashboard.
2. Enter filter a name.
3. Choose the type of filter you want to create. You are able to create a Date, String, Number or Field filter
4. Add a default value if desired. You can choose a basic default value from the drop-down options, or create a more complex default value based on an advanced match
5. Decide which tiles the filter should be applied to and turn them on. Then, choose the field to which the value of the filter will be applied.
6. For tiles based on merge query results, select the query or queries you want to apply the filter to and turn them on, then select the LookML field to which the filter    value will be applied.
7. In the Filters to Update tab, you can make different filters dependent on the selected filter. To do so:
	* Save your filter, as defined so far.
	* Turn on the switch next to the other filters you want to make dependent on this filter.
8. In the Customize Filter tab, choose the behavior of your filter:
	* Require a filter value to run this dashboard: The user must enter a filter value before the dashboard can be run. 
	* Allow multiple filter values: When this is on, the user can select multiple filter values. When this is off, the user is able to select only a single filter             value.
9. Save your filter


### 7. Copy Of Existing Dashboard and Editing the dashboard <span id="copy1"><span>
	
1. Click on Edit Dashboard and Rename Dashboard and start editing it.
1. Add tiles and filters based on the needed to the edited dashboard.

![copyofnew](copyofnew.PNG)

### 8. Users and Roles of access of dashboards <span id="userroles"><span>

Organizational data contains more sensitiive information and these kind of  visualization dashboards need to be shared to only intended persons.

![roles](roles.PNG)

1. Personal Folder has all the dashboard built from elysium for personal space.
1. Group Folder we can move dashboards from personal to group so that specific User related can view those dashboards.
1. Shared Dashboards will be accessed by all  the users who has access to Elysium applications.

### 9. Dashboards Available in Elysium Analytics <span id="availabledashboards"><span>
	1. Insider Threat Detection
	2. Security Posture
	3. UEBA
	4. Alerts
	5. 360 View Matters
	6. SOC Dashboard
	7. Statistical Dashboard
	8. SOX IT Compliance
	9. HIPAA
	10. NIST
	11. Operational Dashboards
	12. Source Analytics Dashboard
	13. Identity Management 
	14. User session Tracking information
	15. Active Sync and Outlook Web Access

## 6.2 Elysium kibana data visualizations  <span id="kibanaviz1"><span>

To create a visualization:

1. Click on Visualize in the side navigation.
1. Click the Create new visualization button or the + button.
1. Choose the visualization type:

![visua](visualization1.png)

![visu](visualization2.gif)

- Basic charts
  ----
* Line, Area and Bar charts	: Compare different series in X/Y charts
* Heat maps 			: Shade cells within a matrix
* Pie chart 			: Display each source’s contribution to a total

- Data
  -----
* Data table  : Display the raw data of a composed aggregation.
* Metric :  Display a single number.
* Goal and Gauge : Display a gauge.

- Maps
  -----
* Coordinate map: Associate the results of an aggregation with geographic locations.
* Region map : Thematic maps where a shape’s color intensity corresponds to a metric’s value. locations.

- Time Series
  -----
* Timelion : Compute and combine data from multiple time series data sets.
* Time Series Visual Builder: Visualize time series data using pipeline aggregations.

- Other visualizations
  ----
* Controls :Controls provide the ability to add interactive inputs to Kibana Dashboards.
* Markdown widget: Display free-form information or instructions.
* Tag cloud: Display words as a cloud in which the size of the word correspond to its importance.
* Vega graph :Support for user-defined graphs, external data sources, images, and user-defined interactivity.

4. Specify a search query to retrieve the data for your visualization
   * To enter new search criteria, select the index pattern for the indices that contain the data you want to visualize. This opens the visualization builder with a           wildcard query that matches all of the documents in the selected indices.
   * To build a visualization from a saved search, click the name of the saved search you want to use. This opens the visualization builder and loads the selected query.


5. In the visualization builder, choose the metric aggregation for the visualization’s Y axis

	**Metric Aggregations:** count, average,sum, min, max, standard deviation, unique count, median (50th percentile), percentiles, percentile ranks, top hit, geo 	                                   centroid
	**Parent Pipeline Aggregations:** derivative,cumulative sum,moving average, serial diff
	**Sibling Pipeline Aggregations:** average bucket, sum bucket, min bucket, max bucket

6. For the visualizations X axis, select a bucket aggregation:
   Date histogram, range,terms,filters, significant terms

	For example, indexing Apache server logs, visualization of bar chart shows that distribution of incoming requests by geographic location by specifying a terms           aggregation on the geo.src field:
![v2](bar-terms-agg.jpg)

	* The y-axis shows the number of requests received from each country, and the countries are displayed across the x-axis.
	* Bar, line, or area chart visualizations use metrics for the y-axis and buckets for the x-axis. Buckets are analogous to SQL GROUP BY statements. Pie charts,             use the metric for the slice size and the bucket for the number of slices.
	* You can further break down the data by specifying sub aggregations. The first aggregation determines the data set for any subsequent aggregations. Sub           	   aggregations are applied in order.
	* For example, you could add a terms sub aggregation on the geo.dest field to the Country of Origin bar chart to see the locations those requests were targeting
	
![v3](bar-terms-subagg.jpg)




## 6.3 Build Kiabana Dashboards   <span id="mainkibanadashboard"><span>

### Visualize your data with dashboards  <span id="yourdashboard"><span>
* The best way to understand your data is to visualize it. With dashboards, you can turn your data from one or more index patterns into a collection of panels that bring clarity to your data, tell a story about your data, and allow you to focus on only the data that’s important to you. Configure each panel to display your data in a chart, table, map, and more, then compare the panels side-by-side to identify the patterns and connections in your data.	
* User need to have insufficient privileges to create or save dashboards or  Granting access to Kibana.

![dashboard](Dashboard_example.png)

### Open the dashboard  <span id="opendashboard"><span>
Begin with an empty dashboard, or open an existing dashboard.

1.Open the main menu, then click Dashboard.
1. On the Dashboards page, choose one of the following options:
	* To start with an empty dashboard, click Create dashboard.
	* To open an existing dashboard, click the dashboard Title you want to open.

### Create panels   <span id="createpanels"><span>
Choose the type of panel to create, then save the panel to the dashboard.

1. From the dashboard, choose one of the following options:

	* To create a panel, click Create panel, then click the panel type on the New visualization window. Lens is recommended for most users.
	* To add a saved panel, click Add from library, then select the panel you want to add. When a panel contains a stored query, both queries are applied.
1. To save the panel, click Save in the toolbar, then configure the Save visualization options.

	* Enter the Title and optional Description.
	* From the Tags drop down, select any applicable tags.
	* Select Add to Dashboard after saving.
	* Click Save and return.


### clone panels     <span id="clonepanels"><span>
To duplicate a panel and the configured functionality, clone the panel. Cloned panels continue to replicate all of the functionality from the original panel, including renaming, editing, and cloning. When you clone a panel, the clone appears beside the original panel, and moves other panels to provide a space on the dashboard.
1. From the toolbar, click Edit.
1. Open the panel menu, then select Clone panel.

![clone](clone_panel.gif)

### Explore the underlying documents     <span id="exploredocuments"><span>
Dashboard panels have a shortcut to view the underlying documents in Discover. Open the panel menu, then click Explore underlying data. Discover will be opened with the same time range and filters as the panel.

![datacontexting](explore_data_context_menu.png)

* Explore underlying data is available only for visualization panels with a single index pattern.


### Download panel data as CSV     <span id="downloadpanel"><span>
Download panel data in a CSV file. You can download most panels in a CSV file, but there is a shortcut available for Lens panels.

Lens
Open the Lens panel menu, then select More > Download as CSV.

![csv](download_csv_context_menu.png)

![csv1](Dashboard_inspect.png)


### Share the dashboard         <span id="sharedashboard"><span>
To share the dashboard with a larger audience, click Share in the toolbar, then choose one of the following options:

1. Permalinks: Share a direct link to a Kibana dashboard. User authentication is required.
1. PDF Reports: Generate a PDF report.
1. PNG Reports: Generate a PNG report
1. Embed code:  Embed the dashboard as an iframe on a web page. Embedded dashboards are fully interactive, but you can hide some parts of the dashboard using the menu                   options. User authentication is required,


### Export the dashboard    <span id="exportdashboard"><span>
To automate Kibana, you can export dashboards as JSON using the import and export dashboard APIs. It is important to export dashboards with all references needed.


## 8. Data Collection and Ingestion :  <span id="datacolection"><span>


*   Elysium Analytics provides a scalable, robust and flexible architecture, delivered as a service, that assures secure and reliable collection, parsing and loading of 	any type of log data as well as network traffic data into a cloud scale data lake built on top of Snowflake’s data warehouse.
*   Elysium SaaS solution is truly a cloud scale security analytics platform that removes the barriers from
	ingesting, contextualizing, searching, analyzing, and storing log data with a cost-effective and low-risk service

*  Elysium SaaS offering licensed on a usage basis, lowering cost and removing financial risk and provides a low price for storage, and compute is billed by the minute 	of usage.
*   Additionally, Elysium provides open platform with no vendor lock-in, customizable analytics models, as well as APIs for end user development of analytics models.

*   Elysium supports, developed a broad library of Collectors, Parsers and Plug-ins that allows you to collect and load all security related data as well as data for 		context and enrichment into our data lake. Our data collection is delivered as a cloud service; all you need to do is to point your data sources to our 		infrastructure and we will take of it from there.


![maincollection](maincollection.png)

## 1. Collect your data/ Shippers   <span id="shippers"><span>

With integration to all your security and log sources, Elysium Analytics automatically collects all the data you need from any source; cloud, on-prem, or SIEM solution. Leveraging Kafka, Logstash, Beats, and Nifi.

Collect all your enterprise network and endpoint device logs for full visibility to all activity across all layers of your
network.

Collect all log data from your all your security devices, on-premises and cloud implementations for a consolidated view of all activity across all your security solutions and retain the data for as long as you need to.

![operational](operationalmain.PNG)

**Elysium Beats**

* Elysium Beats are a set of lightweight data shippers that allow to conveniently send data to data lake Service. 
* Being lightweight, Beats do not incur much runtime overhead and they can therefore run and collect data on devices with limited hardware resources, such as IoT      		devices, edge device, or embedded devices. 
* Beats are the perfect match if you need to collect data without having the resources to run resource-intensive data collectors. This kind of pervasive data collection on all of your networked devices allows you to quickly detect and react upon, for example, system-wide issues and security incidents.Of course, Beats are not limited to resource-constrained systems. They can also be used on systems that have more hardware resources available.

**The Beats fleet: an overview** 
Beats come in various flavors to collect different kinds of data:

* There are numerous ways to ingest data into elysium Service. The choice of specific methods or tools to ingest data depends on your specific use case, requirements, and environment.
* Beats provide a convenient and lightweight out-of-the-box solution to collect and ingest data from many different sources.
* Packaged with the Beats are modules that provide the configuration for data acquisition, parsing, indexing, and visualization for many common databases, operating systems, container environments, web servers, caches, and so on.


![beats](beats1.PNG)
 
**Logstash**

* Logstash is a powerful and flexible tool to read, process, and ship data of any kind and integrates the data from different external sources.
* A common architectural pattern is to combine Beats and Logstash: use Beats to collect data and use Logstash to perform any data processing that Beats are not capable   of doing.
* Logstash works by executing event processing pipelines, whereby each pipeline consists of at least one of each of the following:

	1. Inputs:  read from data sources. Many data sources are officially supported, including files, http, imap, jdbc, kafka, syslog, tcp, and udp.
	2. Filters: process and enrich the data in various ways. In many cases, unstructured log lines first need to be parsed into a more structured format. Logstash 		    therefore provides, among others, filters to parse CSV, JSON, key/value pairs, delimited unstructured data, and complex unstructured data on the basis 		    of regular expressions (grok filters). Logstash further provides filters to enrich data by performing DNS lookups, adding geoinformation about IP 			    addresses, or by performing lookups against a custom dictionary. Additional filters allow for diverse transformations of the data, for example, to rename, 			remove, copy data fields and values (mutate filter).
	3.  Outputs: write the parsed and enriched data to data sinks and are the final stage of the Logstash processing pipeline.


```bash
Logstash Config file:
input {
  file {
         path => "/var/log/apache2/access.log"
    start_position => "beginning"
    sincedb_path => "/dev/null"
  }
}
filter {
    grok {
      match => { "message" => "%{COMBINEDAPACHELOG}" }
    }
    date {
    match => [ "timestamp" , "dd/MMM/yyyy:HH:mm:ss Z" ]
  }
  geoip {
      source => "clientip"
    }
}
output {
  elysiumsearch {
    hosts => ["localhost:9200"]
  }
}


```

The following Eysium Data collection dashboards describes the sum of ingeated count by source, Total count of events per host, Data Collection for last 24 Hours and it can also provides filter the data collection events using time intervals.
 
![datacollection](datacollection1.PNG)


![datacollection2](datacollection2.PNG)
 
## 2. Connect to your data (Connectors and plugins)      <span id="connectyourdata"><span>
* Combine all your on-prem IT logs, enterprise network logs, cloud logs and network traffic data into one scalable data lake and combine your in-cloud and on-prem data silos into one scalable Snowflake data lake.

* Elysium connectors and plugins reduces the  client configuration setups requirements  to collect the data from various log sources.

![awsconnectors](aws.PNG)

![cloudapps1](cloudapps1.PNG)

![microsoftconnectors](microsoft1.PNG)

**create custom connectors:**
Elysium connectors allow users and provides flexibility  to create own connectors to collect the data.
![createconnector](createconnector.PNG)


**Elysium Plugins**

|Plugin|Description|
|:---------|:--------|
|azure_event_hubs| Receives events from Azure Event Hubs|
|beats|Receives events from the Elastic Beats framework|
|cloudwatch|Pulls events from the Amazon Web Services CloudWatch API|
|couchdb_changes|Streams events from CouchDB’s _changes URI|
|dead_letter_queue|read events from Logstash’s dead letter queue|
|elasticsearch|Reads query results from an Elasticsearch cluster|
|exec|Captures the output of a shell command as an event|
|file|Streams events from files|
|ganglia|Reads Ganglia packets over UDP|
|gelf|Reads GELF-format messages from Graylog2 as events|
|generator|	Generates random log events for test purposes|
|github|Reads events from a GitHub webhook|
|google_cloud_storage|	Extract events from files in a Google Cloud Storage bucket|
|google_pubsub|	Consume events from a Google Cloud PubSub service|
|graphite|Reads metrics from the graphite tool|
|heartbeat|Generates heartbeat events for testing|
|http|	Receives events over HTTP or HTTPS|
http_poller|Decodes the output of an HTTP API into events
|imap|	Reads mail from an IMAP server|
|irc|	Reads events from an IRC server|
|java_generator|	Generates synthetic log events|
|java_stdin|	Reads events from standard input|
|jdbc|	Creates events from JDBC data|
|jms|	Reads events from a Jms Broker|
|jmx|	Retrieves metrics from remote Java applications over JMX|
|kafka|	Reads events from a Kafka topic|
|kinesis|	Receives events through an AWS Kinesis stream|
|log4j|	Reads events over a TCP socket from a Log4j SocketAppender object|
|lumberjack|	Receives events using the Lumberjack protocl|
|meetup|	Captures the output of command line tools as an event|
|pipe|	Streams events from a long-running command pipe|
|puppet_facter|	Receives facts from a Puppet server|
|rabbitmq|	Pulls events from a RabbitMQ exchange|
|redis|	Reads events from a Redis instance|
|relp|	Receives RELP events over a TCP socket|
|rss|	Captures the output of command line tools as an event|
|s3|	Streams events from files in a S3 bucket|
|salesforce|	Creates events based on a Salesforce SOQL query|
|snmp|	Polls network devices using Simple Network Management Protocol (SNMP)|
|snmptrap|	Creates events based on SNMP trap messages|
|sqlite|	Creates events based on rows in an SQLite database|
|sqs|	Pulls events from an Amazon Web Services Simple Queue Service queue|
|stdin|	Reads events from standard input|
|stomp|	Creates events received with the STOMP protocol|
|syslog|	Reads syslog messages as events|
|tcp|	Reads events from a TCP socket|
|twitter|	Reads events from the Twitter Streaming API|
|udp|	Reads events over UDP|
|unix|	Reads events over a UNIX socket|
|varnishlog|	Reads from the varnish cache shared memory log|
|websocket|	Reads events from a websocket|
|wmi|	Creates events based on the results of a WMI query|
|xmpp|	Receives events over the XMPP/Jabber protocol|


## 3. Parse your data              <span id="parsedata"><span>
Parse, map, and group your data, in Elysium Analytics Open Data Model for full context and fast, analytics.
Parse legacy device data sources in Logstash and modern data sources using different kind of suppoted formats.

|Parser Name| Description|
|:---------|:--------|
|MSFT Exchange|	 Microsoft email events|
|Windows Audit|	Windows audit and sysmon events|
|Bluecoat|	Web proxy events|
|WatchGuard - DNS|	Web proxy DNS events|
|WatchGuard - VPN|	Web proxy VPN events|
|Cisco ASA|	Firewall and VPN events|
|Windows Sysmon|	Windows system monitoring events|
|Symantec Endpoint Protection|	Anti-virus events|
|Barracuda|	Web email events|
|Palo Alto|	Firewall, Proxy and VPN events|
|Web Sphere|	Web traffic events|
|FireEye|	 Web download traffic inspection events|
|Source Fire|	IDS events|
|Bro/Zeek|	Flow data|
|Snort IDS|	IDS events|
|Netflow, IPFIX	|  Flow data|
|AWS|	Cloud security events|
|Azure|	Cloud security events|
|AS/400 and iSeries|	Mainframe|
|Box|	Cloud services|
|Checkpoint OPSEC/LEA|	Firewall and VPN events|
|Cisco SDEE|	Content delivery events|
|Cloud/SaaS solutions|	Cloud events|
|Cradlepoint|	Network edge events|
|Flat files (single-line and multi-line, compressed or uncompressed)|	Custom flat file events|
|Flex Database Log Adapter for system and custom logs written to database tables(e.g.,Oracle, SQL Server,MySQL)(ODBC & JDBC protocols)|Custom db events|
|Flow data (e.g., IPFIX, NetFlow, sFlow, J-Flow, SmartFlow) |   Flow data|
|McAfee A/V|	Anti-virus events|
|McAfee HIPS|	Endpoint monitoring events|
|MSFT IIS|	Web traffic events|
|Netflow, IPFIX	|    Flow data|
|Office 365|	Microsoft Office 365 events|
|Qualys |  	Vulnerability events|
|Rapid7	|  Collectoin of web proxy events|
|Redhat |   Enterprise OS events|
|Salesforce|	CRM vents|
|SNMP|	Traps event|
|Snort IDS|	IDS events|
|Sourcefire eStreamer| IDS streaming events|
|Squid|	Web proxy events|
|Symantec DLP|	DLP events|
|Tenable Security Center|	 Security events|
|UDP/TCP and secure syslog|	Custom network events|
|Vendor-specific APIs (example sources)|	Collectoin of web proxy events|
|Vulnerability scanners (example sources)|	Vulnerability events|
|Vendor-specific APIs (example sources)|	Collectoin of web proxy events|
|Vulnerability scanners (example sources)|	Vulnerability events|



## 4. Enrich your data                <span id="enrichdata"><span>

Enrich data in real time with Identity, Asset, Geolocation,Threat Intelligence, as well as data from lookup tables built into the storage platform data
pipeline.

Context enrichment adds event and non-event contextual information to security event data in order to transform raw data into meaningful insights. User typically enrich with geo data, asset lookup data, and more.

It has three prerequisites before you can use it in your pipeline:
* you need to have the source index from which we will get the enrichment data
* you need to define an enrich policy defining source indices, matched field and the appended fields
* you need to _execute the enrich policy to create an enrich index for the policy


## 5. Load your data        <span id="loaddata"><span>
* Data lake is billed by the second and can be configured to continuous loading or batch loading. 
* Elysium SaaS provides a low price for storage when compared to other log analysis vendors. 
* Elysium Analytics is running on Snowflake’s Data Cloud with
separation of storage and compute. This is a major breakthrough as users can scale storage and
compute completely independently and transparently as needed.
* consider a case where there is a need to ingest 2TB of log data daily and retain
the data for one year which adds up to 720TB ingested data. With Elysium Analytics, we will provide
collection, parsing and loading (ELT) as a service.

|Elysium Analytics cost|AWS Ultrawarm cost|Traditional Elasticsearch cost|
|:---------|:--------|:---------|
|Loading compute cost: $2,344|3 master nodes r5.2xl: $1,057|3 master nodes r5.2xl:$ 2,117
|Storage compressed 10X: $1,656|37 Ultrawarm nodes: $70,416|132 data nodes i3.16xl:$ 502,396
|Query compute cost:$2,160|720TB managed storage: $17,280|
|Total monthly cost:$6,160| Total monthly cost: $88,753|Total monthly cost:$ 504,513










## 6. Add Threat Intelligence to your data         <span id="addthreat"><span>

Enrich your data with Threat Intel and get a broad view of the threat landscape external to your organization allowing your security
team to more effectively detect threats, measure overall relevant risk exposure, and become more effective at mitigation.
We have implemented a RESTful API as well as STIX & TAXII support for simple ingestion into our data lake.


## 7. Cloud Apps              <span id="cloudapps"><span>
Collect, aggregate and analyze logs from any cloud application source. Simple setup, get insights  from all your cloud applications, infrastructure, and devices.
	
	
![cloudconnectors](cloudapps.PNG)

## 8. Data Investigation Dashboards        <span id="investigationdashboard"><span>

Data Investigation dashboards represents data stream processing of statistics, counts by each source, min, max, average time in hours to process events.
It also provides time delay Notfications, alerts during failures of ingestion of data. 
	
![dataingestion](dataingestion.PNG)
	
![dataingestion2](dataingestion2.PNG)	
	
## 9. Data Ingestion tracking         <span id="ingestiontracking"><span>

Data Ingestion Tracking dashboard provides aggregation of date, Source name, type, host  of events list 


![datatracking](datatracking.PNG)	


## 10. Logstash Network Traffic Dashboards   <span id="LogstashNetwork"><span>

![logstash1.PNG](logstash1.PNG)






## 6. Alerts tiles

Overview of alert  tiles in the Dashboard

1.  New Alerts  
     It shows the everyday count of alerts.Click on the graph  Show All,Drill appears
     Click on Drill into any of the event time  it takes to the Details.
2.  New Alerts By Severity 
     It shows the count of alerts per severity.Low,high Critical are level of Severity.Click on 
     the graph Show All, Filter By Severity appears.Click on Filter By Severity it redirects
     to Dashboard with severity value as filter.
3.  New Alerts By Type 
     It shows the count of alerts according to the alert names.Different colored bars represent
     to  the  respective alert abbreviation names .Click on the graph Show All,
     Filter By Alert name appears. Click on the Filter By Alert name it filters with the alert_name.
4.  Alerts By Source 
     It shows the count of alerts according to the source names.Different colored lines 
     represent the respective Source names .
5.  Alerts Origination From Geo 
     It shows the count of Alerts per Location.
6.  Alert  types for last 7 days
     It  shows the different alerts types,count of alerts and alerts generated date. Click on graph 
     Filter By Alert Name  appears. Click on Filter By Alert Name it redirects to the Dashboard by 
     filtering  alert name.
7.  User Alerts for 7 days 
     It shows the name of the user,count of alerts,alerts generated date.
8.  Alerts Data 
     It shows the information of count of alerts,alert type,description,alert abbreviation name,
     user name ,event time minute and total count of alerts.
9.  Detailed View 
     It shows information about  alerts,ID,Parent Alert ID,user name,source,IP’ s of both source 
     and destination, Hostname
 

## 7. Statistical Data / Information

Filter: User can change the filter and run the dashboard 


Overview of the Tiles in Dashboard

City shows the Count of Events per City
Total Activity Per Region shows the total Events / Activities per City per day
Bandwidth Usage/City shows the  Total uploaded and downloaded bytes per City
Top 10 Users/ Bandwidth shows the first 10 users who used the most Bandwidth (sum of uploaded and downloaded bytes)
Details shows the details of a particular user / system like Name, City, Event Date, Successful Login, Number of Emails etc.
If you hover over (1-4) tiles, you can see the details like Event Date, City, Bandwidth etc

# 7.  SOC Dashboard
 
Overview of the Tiles in Dashboard

1. Top 10 Alerts shows the count of highest Alerts Types
1. Top Alerts last 48 hours shows the list of users / system with high Alert count with Alert abbreviation name (Alert Type)
1.Alert Count shows the Total count of Alerts.
1. Events Count shows the Total Ingested count
	(1-4) Tiles shows the data in the past 2 days
1. Data Source loading over the last 7 days shows the sum of Ingested count per Source 
1. Top 10 bandwidth Usage shows top 10 users who has uploaded or downloaded the highest amount(Bytes) of data
1. Top 10 Risky Entities shows the high Risk entities
1. Top 10 Risky Users shows the  high Risk Users
1. UEBA’s Sparkline shows the maximum score of the Reports 
	Tiles (5,6 & 9) shows last 7 days of data
	Tiles (7 & 8) shows last 15 days of data with Risk Score >=50
 


## 7. Data Collection and Ingestion (#datacolection)

1. Collect your data/Shippers(#shippers)
2. Connectors and plugins (#connectyourdata)
3. Parsing data(#parsedata)
4. Enrich data(#enrichdata)
5. Loading data(#loaddata)
6. Add Threat intelligence to your data(#addthreat)
7. Cloud Apps (#cloudapps)
8. Data Investigation Dashboards(#investigationdashboard)
9. Data Ingestion tracking(#ingestiontracking)
10. Logstash Network Traffic Dashboards(#LogstashNetwork)
