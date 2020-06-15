---
output: hugodown::md_document
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "DT table"
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
rmd_hash: 9a3ca526e9cebbe0
html_dependencies:
- <script src="htmlwidgets-1.5.1/htmlwidgets.js"></script>
- <script src="jquery-1.12.4/jquery.min.js"></script>
- <link href="datatables-css-0.0.0/datatables-crosstalk.css" rel="stylesheet" />
- <script src="datatables-binding-0.13/datatables.js"></script>
- <link href="dt-core-1.10.20/css/jquery.dataTables.min.css" rel="stylesheet" />
- <link href="dt-core-1.10.20/css/jquery.dataTables.extra.css" rel="stylesheet" />
- <script src="dt-core-1.10.20/js/jquery.dataTables.min.js"></script>
- <link href="crosstalk-1.1.0.1/css/crosstalk.css" rel="stylesheet" />
- <script src="crosstalk-1.1.0.1/js/crosstalk.min.js"></script>

---

DT
==

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
<span class='c'>#&gt;  - attr(*, "class")= chr "html_dependency"</span>
<span class='nf'>library</span>(<span class='k'><a href='https://rdrr.io/pkg/DT/man'>DT</a></span>)
<span class='nf'><a href='https://rdrr.io/pkg/DT/man/datatable.html'>datatable</a></span>(<span class='k'>Orange</span>)
<!--html_preserve--><div id="htmlwidget-37ddcb8437de4fd72419" style="width:100%;height:auto;" class="datatables html-widget"></div>
<script type="application/json" data-for="htmlwidget-37ddcb8437de4fd72419">{"x":{"filter":"none","data":[["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","33","34","35"],["1","1","1","1","1","1","1","2","2","2","2","2","2","2","3","3","3","3","3","3","3","4","4","4","4","4","4","4","5","5","5","5","5","5","5"],[118,484,664,1004,1231,1372,1582,118,484,664,1004,1231,1372,1582,118,484,664,1004,1231,1372,1582,118,484,664,1004,1231,1372,1582,118,484,664,1004,1231,1372,1582],[30,58,87,115,120,142,145,33,69,111,156,172,203,203,30,51,75,108,115,139,140,32,62,112,167,179,209,214,30,49,81,125,142,174,177]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>Tree<\/th>\n      <th>age<\/th>\n      <th>circumference<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"columnDefs":[{"className":"dt-right","targets":[2,3]},{"orderable":false,"targets":0}],"order":[],"autoWidth":false,"orderClasses":false}},"evals":[],"jsHooks":[]}</script><!--/html_preserve--></code></pre>

</div>

