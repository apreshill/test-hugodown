---
output: hugodown::md_document
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "highcharter"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2020-06-09"
lastmod: 2020-06-09
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
rmd_hash: 3611bcdd187a9290
html_dependencies:
- <script src="htmlwidgets-1.5.1/htmlwidgets.js"></script>
- <script src="jquery-1.11.1/jquery.min.js"></script>
- <script src="proj4js-2.3.15/proj4.js"></script>
- <link href="highcharts-7.0.1/css/motion.css" rel="stylesheet" />
- <link href="highcharts-7.0.1/css/htmlwdgtgrid.css" rel="stylesheet" />
- <script src="highcharts-7.0.1/highcharts.js"></script>
- <script src="highcharts-7.0.1/highcharts-3d.js"></script>
- <script src="highcharts-7.0.1/highcharts-more.js"></script>
- <script src="highcharts-7.0.1/modules/stock.js"></script>
- <script src="highcharts-7.0.1/modules/map.js"></script>
- <script src="highcharts-7.0.1/modules/annotations.js"></script>
- <script src="highcharts-7.0.1/modules/boost.js"></script>
- <script src="highcharts-7.0.1/modules/data.js"></script>
- <script src="highcharts-7.0.1/modules/drag-panes.js"></script>
- <script src="highcharts-7.0.1/modules/drilldown.js"></script>
- <script src="highcharts-7.0.1/modules/item-series.js"></script>
- <script src="highcharts-7.0.1/modules/offline-exporting.js"></script>
- <script src="highcharts-7.0.1/modules/overlapping-datalabels.js"></script>
- <script src="highcharts-7.0.1/modules/exporting.js"></script>
- <script src="highcharts-7.0.1/modules/export-data.js"></script>
- <script src="highcharts-7.0.1/modules/funnel.js"></script>
- <script src="highcharts-7.0.1/modules/heatmap.js"></script>
- <script src="highcharts-7.0.1/modules/treemap.js"></script>
- <script src="highcharts-7.0.1/modules/sankey.js"></script>
- <script src="highcharts-7.0.1/modules/solid-gauge.js"></script>
- <script src="highcharts-7.0.1/modules/streamgraph.js"></script>
- <script src="highcharts-7.0.1/modules/sunburst.js"></script>
- <script src="highcharts-7.0.1/modules/vector.js"></script>
- <script src="highcharts-7.0.1/modules/wordcloud.js"></script>
- <script src="highcharts-7.0.1/modules/xrange.js"></script>
- <script src="highcharts-7.0.1/modules/tilemap.js"></script>
- <script src="highcharts-7.0.1/modules/venn.js"></script>
- <script src="highcharts-7.0.1/modules/gantt.js"></script>
- <script src="highcharts-7.0.1/modules/timeline.js"></script>
- <script src="highcharts-7.0.1/modules/parallel-coordinates.js"></script>
- <script src="highcharts-7.0.1/plugins/grouped-categories.js"></script>
- <script src="highcharts-7.0.1/plugins/motion.js"></script>
- <script src="highcharts-7.0.1/plugins/multicolor_series.js"></script>
- <script src="highcharts-7.0.1/custom/reset.js"></script>
- <script src="highcharts-7.0.1/custom/symbols-extra.js"></script>
- <script src="highcharts-7.0.1/custom/text-symbols.js"></script>
- <script src="highchart-binding-0.7.0/highchart.js"></script>

---

<div class="highlight">

<pre class='chroma'><code class='language-r' data-lang='r'><span class='k'>htmltools</span>::<span class='nf'><a href='https://rdrr.io/pkg/htmltools/man/suppressDependencies.html'>suppressDependencies</a></span>(<span class='s'>"jquery"</span>)[[<span class='m'>1</span>]]
<span class='c'>#&gt; character(0)</span>
<span class='c'>#&gt; attr(,"html_dependencies")</span>
<span class='c'>#&gt; attr(,"html_dependencies")[[1]]</span>
<span class='c'>#&gt; List of 10</span>
<span class='c'>#&gt;  $ name      : chr "jquery"</span>
<span class='c'>#&gt;  $ version   : chr "9999"</span>
<span class='c'>#&gt;  $ src       :List of 1</span>
<span class='c'>#&gt;   ..$ href: chr ""</span>
<span class='c'>#&gt;  $ meta      : NULL</span>
<span class='c'>#&gt;  $ script    : NULL</span>
<span class='c'>#&gt;  $ stylesheet: NULL</span>
<span class='c'>#&gt;  $ head      : NULL</span>
<span class='c'>#&gt;  $ attachment: NULL</span>
<span class='c'>#&gt;  $ package   : NULL</span>
<span class='c'>#&gt;  $ all_files : logi TRUE</span>
<span class='c'>#&gt;  - attr(*, "class")= chr "html_dependency"</span></code></pre>

</div>

Highcharter
-----------

<div class="highlight">

<pre class='chroma'><code class='language-r' data-lang='r'><span class='nf'>library</span>(<span class='k'><a href='https://rdrr.io/pkg/highcharter/man'>highcharter</a></span>)
<span class='c'>#&gt; Registered S3 method overwritten by 'quantmod':</span>
<span class='c'>#&gt;   method            from</span>
<span class='c'>#&gt;   as.zoo.data.frame zoo</span>
<span class='c'>#&gt; Highcharts (www.highcharts.com) is a Highsoft software product which is</span>
<span class='c'>#&gt; not free for commercial and Governmental use</span>
<span class='nf'><a href='https://rdrr.io/pkg/highcharter/man/hchart.html'>hchart</a></span>(<span class='k'>Orange</span>, <span class='s'>"line"</span>, <span class='nf'><a href='https://rdrr.io/pkg/highcharter/man/hcaes.html'>hcaes</a></span>(x = <span class='k'>age</span>, y = <span class='k'>circumference</span>, group = <span class='k'>Tree</span>))
<span class='c'>#&gt; Warning: `parse_quosure()` is deprecated as of rlang 0.2.0.</span>
<span class='c'>#&gt; Please use `parse_quo()` instead.</span>
<span class='c'>#&gt; <span style='color: #555555;'>This warning is displayed once per session.</span></span>
<span class='c'>#&gt; Warning: `group_by_()` is deprecated as of dplyr 0.7.0.</span>
<span class='c'>#&gt; Please use `group_by()` instead.</span>
<span class='c'>#&gt; See vignette('programming') for more help</span>
<span class='c'>#&gt; <span style='color: #555555;'>This warning is displayed once every 8 hours.</span></span>
<span class='c'>#&gt; <span style='color: #555555;'>Call `lifecycle::last_warnings()` to see where this warning was generated.</span></span>
<span class='c'>#&gt; Warning: `select_()` is deprecated as of dplyr 0.7.0.</span>
<span class='c'>#&gt; Please use `select()` instead.</span>
<span class='c'>#&gt; <span style='color: #555555;'>This warning is displayed once every 8 hours.</span></span>
<span class='c'>#&gt; <span style='color: #555555;'>Call `lifecycle::last_warnings()` to see where this warning was generated.</span></span>
<span class='c'>#&gt; Warning: `as_data_frame()` is deprecated as of tibble 2.0.0.</span>
<span class='c'>#&gt; Please use `as_tibble()` instead.</span>
<span class='c'>#&gt; The signature and semantics have changed, see `?as_tibble`.</span>
<span class='c'>#&gt; <span style='color: #555555;'>This warning is displayed once every 8 hours.</span></span>
<span class='c'>#&gt; <span style='color: #555555;'>Call `lifecycle::last_warnings()` to see where this warning was generated.</span></span>
<span class='c'>#&gt; Warning: `rename_()` is deprecated as of dplyr 0.7.0.</span>
<span class='c'>#&gt; Please use `rename()` instead.</span>
<span class='c'>#&gt; <span style='color: #555555;'>This warning is displayed once every 8 hours.</span></span>
<span class='c'>#&gt; <span style='color: #555555;'>Call `lifecycle::last_warnings()` to see where this warning was generated.</span></span>
<!--html_preserve--><div id="htmlwidget-baaebe6f3a6634e860c0" style="width:100%;height:500px;" class="highchart html-widget"></div>
<script type="application/json" data-for="htmlwidget-baaebe6f3a6634e860c0">{"x":{"hc_opts":{"title":{"text":null},"yAxis":{"title":{"text":"circumference"},"type":"linear"},"credits":{"enabled":false},"exporting":{"enabled":false},"plotOptions":{"series":{"label":{"enabled":false},"turboThreshold":0,"showInLegend":true},"treemap":{"layoutAlgorithm":"squarified"},"scatter":{"marker":{"symbol":"circle"}}},"series":[{"name":"3","data":[{"Tree":"3","age":118,"circumference":30,"x":118,"y":30},{"Tree":"3","age":484,"circumference":51,"x":484,"y":51},{"Tree":"3","age":664,"circumference":75,"x":664,"y":75},{"Tree":"3","age":1004,"circumference":108,"x":1004,"y":108},{"Tree":"3","age":1231,"circumference":115,"x":1231,"y":115},{"Tree":"3","age":1372,"circumference":139,"x":1372,"y":139},{"Tree":"3","age":1582,"circumference":140,"x":1582,"y":140}],"type":"line"},{"name":"1","data":[{"Tree":"1","age":118,"circumference":30,"x":118,"y":30},{"Tree":"1","age":484,"circumference":58,"x":484,"y":58},{"Tree":"1","age":664,"circumference":87,"x":664,"y":87},{"Tree":"1","age":1004,"circumference":115,"x":1004,"y":115},{"Tree":"1","age":1231,"circumference":120,"x":1231,"y":120},{"Tree":"1","age":1372,"circumference":142,"x":1372,"y":142},{"Tree":"1","age":1582,"circumference":145,"x":1582,"y":145}],"type":"line"},{"name":"5","data":[{"Tree":"5","age":118,"circumference":30,"x":118,"y":30},{"Tree":"5","age":484,"circumference":49,"x":484,"y":49},{"Tree":"5","age":664,"circumference":81,"x":664,"y":81},{"Tree":"5","age":1004,"circumference":125,"x":1004,"y":125},{"Tree":"5","age":1231,"circumference":142,"x":1231,"y":142},{"Tree":"5","age":1372,"circumference":174,"x":1372,"y":174},{"Tree":"5","age":1582,"circumference":177,"x":1582,"y":177}],"type":"line"},{"name":"2","data":[{"Tree":"2","age":118,"circumference":33,"x":118,"y":33},{"Tree":"2","age":484,"circumference":69,"x":484,"y":69},{"Tree":"2","age":664,"circumference":111,"x":664,"y":111},{"Tree":"2","age":1004,"circumference":156,"x":1004,"y":156},{"Tree":"2","age":1231,"circumference":172,"x":1231,"y":172},{"Tree":"2","age":1372,"circumference":203,"x":1372,"y":203},{"Tree":"2","age":1582,"circumference":203,"x":1582,"y":203}],"type":"line"},{"name":"4","data":[{"Tree":"4","age":118,"circumference":32,"x":118,"y":32},{"Tree":"4","age":484,"circumference":62,"x":484,"y":62},{"Tree":"4","age":664,"circumference":112,"x":664,"y":112},{"Tree":"4","age":1004,"circumference":167,"x":1004,"y":167},{"Tree":"4","age":1231,"circumference":179,"x":1231,"y":179},{"Tree":"4","age":1372,"circumference":209,"x":1372,"y":209},{"Tree":"4","age":1582,"circumference":214,"x":1582,"y":214}],"type":"line"}],"xAxis":{"type":"linear","title":{"text":"age"},"categories":null}},"theme":{"chart":{"backgroundColor":"transparent"}},"conf_opts":{"global":{"Date":null,"VMLRadialGradientURL":"http =//code.highcharts.com/list(version)/gfx/vml-radial-gradient.png","canvasToolsURL":"http =//code.highcharts.com/list(version)/modules/canvas-tools.js","getTimezoneOffset":null,"timezoneOffset":0,"useUTC":true},"lang":{"contextButtonTitle":"Chart context menu","decimalPoint":".","downloadJPEG":"Download JPEG image","downloadPDF":"Download PDF document","downloadPNG":"Download PNG image","downloadSVG":"Download SVG vector image","drillUpText":"Back to {series.name}","invalidDate":null,"loading":"Loading...","months":["January","February","March","April","May","June","July","August","September","October","November","December"],"noData":"No data to display","numericSymbols":["k","M","G","T","P","E"],"printChart":"Print chart","resetZoom":"Reset zoom","resetZoomTitle":"Reset zoom level 1:1","shortMonths":["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"],"thousandsSep":" ","weekdays":["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"]}},"type":"chart","fonts":[],"debug":false},"evals":[],"jsHooks":[]}</script><!--/html_preserve--></code></pre>

</div>

