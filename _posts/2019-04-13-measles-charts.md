---
title: "Example: Embedding Altair & Hvplot Charts"
date: 2019-04-13
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Embedding interactive charts on static pages using Jekyll."
altair-loader:
  altair-chart-1: "charts/measlesAltair.json"
  altair-chart-2: "charts/altair_cancellation.json"
hv-loader:
  hv-chart-1: "charts/measlesHvplot.html"
toc: true
toc_sticky: true
---

This post will show examples of embedding interactive charts produced using [Altair](https://altair-viz.github.io) and [Hvplot](https://hvplot.pyviz.org/).

## Altair Example

Below is a chart of the incidence of measles since 1928 for the 50 US states.

<div id="altair-chart-1"></div>

<div id="altair-chart-2"></div>
This was produced using Altair and embedded in this static web page. Note that you can also display Python code on this page:

```python
import altair as alt
alt.renderers.enable('notebook')
```

## Holoviews Example

Lastly, the measles incidence produced using the Holoviews package:

<div id="hv-chart-1"></div>

## Notes

- See the [raw source code](https://raw.githubusercontent.com/nickhand/static-site-template/master/_posts/2019-04-13-measles-charts.md) of this post for details on how these charts were embedded.
- See the [week 13 lecture slides](https://github.com/MUSA-620-Fall-2019/week-13/blob/master/lecture-13.ipynb) for the code that produced these plots.

**Important: When embedding charts, you will likely need to adjust the width/height of the charts before embedding them in the page so they fit nicely when embedded.**
