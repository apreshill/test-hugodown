---
output: hugodown::md_document
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Rmd post with ggplot2"
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
rmd_hash: ca8ac698acc9ebf8

---

<div class="highlight">

<pre class='chroma'><code class='language-r' data-lang='r'><span class='nf'>library</span>(<span class='k'><a href='https://ggplot2.tidyverse.org/reference'>ggplot2</a></span>)
<span class='k'>oplot</span> <span class='o'>&lt;-</span> <span class='nf'><a href='https://ggplot2.tidyverse.org/reference/ggplot.html'>ggplot</a></span>(<span class='k'>Orange</span>, <span class='nf'><a href='https://ggplot2.tidyverse.org/reference/aes.html'>aes</a></span>(x = <span class='k'>age</span>, 
                   y = <span class='k'>circumference</span>, 
                   colour = <span class='k'>Tree</span>)) <span class='o'>+</span>
  <span class='nf'><a href='https://ggplot2.tidyverse.org/reference/geom_point.html'>geom_point</a></span>() <span class='o'>+</span>
  <span class='nf'><a href='https://ggplot2.tidyverse.org/reference/geom_path.html'>geom_line</a></span>() <span class='o'>+</span>
  <span class='nf'><a href='https://ggplot2.tidyverse.org/reference/guides.html'>guides</a></span>(colour = <span class='m'>FALSE</span>) <span class='o'>+</span>
  <span class='nf'><a href='https://ggplot2.tidyverse.org/reference/ggtheme.html'>theme_bw</a></span>()
<span class='k'>oplot</span>
</code></pre>
<img src="figs/unnamed-chunk-1-1.png" width="700px" style="display: block; margin: auto;" />

</div>

