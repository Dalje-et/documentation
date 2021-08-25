---
title: Quick Graphs
kind: documentation
---

## Overview

Quick graphs is a way to graph your data from any page in Datadog. There are three ways to open the Quick graphs editor:

* Press `G` on any page
* The global search (`Cmd+K`) menu
* The dashboards submenu

{{< img src="dashboards/guide/quick_graph_editor.png" alt="quick graph editor" style="width:80%;">}}

## Configuring a graph

To configure your graph on using Quick Graphs, follow this process:

1. Query data
    * [Graphing Metrics](#graphing-metrics)
    * [Graphing Events](#graphing-events)
2. [Select the visualization](#select-your-visualization)
3. [Title the graph](#create-a-title)
4. [Save the graph](#export)

### Query Data

#### Graphing metrics

To query metrics, follow this process outlined in [Dashboard Querying][1]:
1. [Choose the metric to graph][1]
2. [Filter][2]
3. [Aggregate and rollup][3]
4. [Apply additional functions][4]

#### Graphing events
This section provides a brief overview of querying event platform data sources such as [Logs][5], [APM][6], [RUM][7], [Security][8], [Events][9], [CI Pipelines][10], [CI Tests][11], and [Findings][12]. Choose the event data source using the dropdown which is defaulted to **Metrics**. 

To query event data, follow this process:
1. **Filter:** Narrow down, broaden, or shift your focus on the subset of data of current interest. The top field allows you to input a search query mixing key:value and full-text search. 

{{< img src="dashboards/guide/quick_graph_event_filter.png" alt="event filtering" style="width:80%;">}}

2. **Choose the measure or facet:** Measure lets you choose the aggregation function whereas facet displays the unique count. 

{{< img src="dashboards/guide/quick_graph_event_measure.png" alt="choosing measure" style="width:80%;">}}

3. **Aggregate:** If you are graphing a measure, select the aggregation function for the measure you want to graph and use a facet to split your graph.

{{< img src="dashboards/guide/quick_graph_event_group.png" alt="choosing aggregation" style="width:80%;">}}

4. **Rollup:** Choose the time interval for your graph. Changing the global timeframe changes the list of available timestep values.

5. **[Apply additional functions][4]** (same as metrics)

Quick Graphs supports contextual information for logs. With Quick Graphs, you can confirm you are querying and graphing the correct data through our inline data previews and detailed event views. The inline data will open automatically when you select **Logs** and can be closed using the button to the left of your query editor.

{{< img src="dashboards/guide/quick_graph_data_preview.png" alt="quick graph inline data preview"  style="width:80%;">}}

You can click individual log lines to open a detailed view in the [side panel][13].

### Select your visualization


Quick Graphs supports:
* [Timeseries][14]
* [Top List][15]
* [Query value][13]
* [Geomap][16]

### Create a title

If you do not enter a title, one is automatically generated based on your selections. However, it is recommended that you create a title that describes the purpose of the graph.

### Export & Share

Click **Export** to save your work to a Dashboard or Notebook. You can always come back to the editor to change the graph. If want to share a link directly to your graph without a Dashboard or Notebook, click **Copy to Clipboard**.

[1]: dashboards/querying/#choose-the-metric-to-graph
[2]: /dashboards/querying/#filter
[3]: /dashboards/querying/#aggregate-and-rollup
[4]: /dashboards/querying/#advanced-graphing
[5]: /logs/explorer/
[6]: /tracing/trace_search_and_analytics/
[7]: /real_user_monitoring/explorer/search/
[8]: /security_platform/explorer/
[9]: /events/
[10]: /continuous_integration/explore_pipelines/
[11]: /continuous_integration/explore_tests/
[12]: /security_platform/cspm/findings/
[13]: /dashboards/widgets/query_value/
[14]: /dashboards/widgets/timeseries/
[15]: /dashboards/widgets/top_list/
[16]: /dashboards/widgets/geomap/
