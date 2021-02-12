---
layout: default
title: Notebooks (experimental)
parent: Kibana
nav_order: 50
redirect_from: /docs/notebooks/
has_children: false
---

# Kibana notebooks (experimental)

Kibana notebooks have a known issue with [tenants](../security/access-control/multi-tenancy/). If you open a notebook and can't see its visualizations, you might be under the wrong tenant, or you might not have access to the tenant at all.
{: .warning }

A Kibana notebook is an interface that lets you easily combine live visualizations and narrative text in a single notebook interface.

With Kibana notebooks, you can interactively explore data by running different visualizations and share your work with team members to collaborate on a project.

A notebook is a document composed of two elements: Kibana visualizations and paragraphs (Markdown). Choose multiple timelines to compare and contrast visualizations.

Common use cases include creating postmortem reports, designing runbooks, building live infrastructure reports, and writing documentation.


## Get Started with Notebooks

To get started, choose **Kibana Notebooks** in Kibana.

### Step 1: Create a notebook

A notebook is an interface for creating reports.

1. Choose **Create notebook** and enter a descriptive name.
1. Choose **Create**.

![Notebook UI](../../images/notebook.png)

Choose **Notebook actions** to rename, duplicate, or delete a notebook.

### Step 2: Add a paragraph

Paragraphs combine text and visualizations for describing data.

#### Add a markdown paragraph

1. To add text, choose **Add markdown paragraph**.
1. Add rich text with markdown syntax.

![Markdown paragraph](../../images/markdown-notebook.png)

#### Add a visualization paragraph

1. To add a visualization, choose **Add Kibana visualization paragraph**.
1. In **Title**, select your visualization and choose a date range.

![Markdown paragraph](../../images/visualization-notebook.png)

- You can choose multiple timelines to compare and contrast visualizations.

To run and save a paragraph, choose **Run**.

![Output](../../images/output-notebook.png)

You can perform the following actions on paragraphs:

- Add a new paragraph to the top of a report.
- Add a new paragraph to the bottom of a report.
- Run all the paragraphs at the same time.
- Clear the outputs of all paragraphs.
- Delete all the paragraphs.
- Move paragraphs up and down.

## Sample Notebook

![sample notebook](../../images/sample-notebook.png)
