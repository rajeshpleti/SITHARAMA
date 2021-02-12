---
layout: default
title: Reporting
parent: Kibana
nav_order: 20
---


# Reporting

The Open Distro for Elasticsearch Kibana reports feature lets you create PNG, PDF, and CSV reports. To use reports, you must have the correct permissions. For summaries of the predefined roles and the permissions they grant, see the [security plugin](../../security/access-control/users-roles/#predefined-roles).


## Create reports from Discovery, Visualize, or Dashboard

On-demand reports let you quickly generate a report from the current view.

1. From the top bar, choose **Reporting**.
1. For dashboards or visualizations, **Download PDF** or **Download PNG**. From the Discover page, choose **Download CSV**.

   Reports generate asynchronously in the background and might take a few minutes, depending on the size of the report. A notification appears when your report is ready to download.

1. To create a schedule-based report, choose **Create report definition**. Then proceed to [Create reports using a definition](#create-reports-using-a-definition). This option pre-fills many of the fields for you based on the visualization, dashboard, or data you were viewing.


## Create reports using a definition

Definitions let you schedule reports for periodic creation.

1. From the left navigation panel, choose **Reporting**.
1. Choose **Create**.
1. Under **Report settings**, enter a name and optional description for your report.
1. Choose the **Report Source** (i.e. the page from which the report is generated). You can generate reports from the **Dashboard**, **Visualize** or **Discover** pages.
1. Choose your dashboard, visualization, or saved search. Then choose a time range for the report.
1. Choose an appropriate file format for the report.
1. (Optional) Add a header or footer for the report. Headers and footers are only available for dashboard or visualization reports.
1. Under **Report trigger**, choose either **On-demand** or **Schedule**.

   For scheduled reports, choose either **Recurring** or **Cron based**. You can receive reports daily or at some other time interval. Cron expressions give you even more flexiblity. See [Cron expression reference](../../alerting/cron/) for more information.

1. Choose **Create**.
