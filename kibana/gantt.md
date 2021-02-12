---
layout: default
title: Gantt Charts
parent: Kibana
nav_order: 10
---

# Gantt charts

Open Distro for Elasticsearch includes a new Kibana visualization: Gantt charts. These charts show the start, end, and duration of unique events in a sequence. Gantt charts are useful in trace analytics, telemetry, and anomaly detection use cases, where you want to understand interactions and dependencies between various events in a schedule.

For example, consider an index of log data. The fields in a typical set of log data, especially audit logs, contain a specific operation or event with a start time and duration.

To create a Gantt chart, do the following:

1. In the visualizations menu, choose **Create visualization** and **Gantt Chart**.
1. Choose a source for chart (e.g. some log data).
1. Under **Metrics**, choose **Event**. For log data, each log is an event.
1. Select the `**Start Time**` and the **Duration** fields from your data set. The start time is the timestamp for the begining of an event. The duration is the amount of time to add to the start time.
1. Under **Results**, choose the number of events that you want to display on the chart. Gantt charts sequence events from earliest to latest based on start time.
1. Choose **Panel settings** to adjust axis labels, time format, and colors.
1. Choose **Update**.

![Gantt Chart](../../images/kibana-gantt-chart.png)

This Gantt chart the ID for each log on the Y axis. Each bar is a unique event that spans some amount of time. Hover over a bar to see the duration of that event.
