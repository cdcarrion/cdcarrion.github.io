---
title: "test5"
output:
  md_document:
    variant: gfm
    preserve_yaml: TRUE
knit: (function(inputFile, encoding) {
   rmarkdown::render(inputFile, encoding = encoding, output_dir = "C:/Users/crist/Documents/GitHub/svmiller.github.io/_posts") })
author: "Cristian"
date: '2020-04-06'
always_allow_html: true
htmlwidgets: TRUE
excerpt: "Here is some R code"
layout: post
categories:
  - R
---

## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax
for authoring HTML, PDF, and MS Word documents. For more details on
using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document. You can embed an R code chunk like this:

``` r
summary(cars)
```

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

## Including Plots

You can also embed plots, for example:

``` r
x <- c(1:100)
random_y <- rnorm(100, mean = 0)
data <- data.frame(x, random_y)

#py = plotly("RgraphingAPI", "ektgzomjbx")
#py$ggploty(plot1, session="knitr")
plot1 = plot_ly(data, x = ~x, y = ~random_y, type = 'scatter', mode = 'lines')

plot1
```

<!--html_preserve-->

<div id="htmlwidget-d6e5713ef85836d93c88" class="plotly html-widget" style="width:2100px;height:1500px;">

</div>

<script type="application/json" data-for="htmlwidget-d6e5713ef85836d93c88">{"x":{"visdat":{"85b81c0246f8":["function () ","plotlyVisDat"]},"cur_data":"85b81c0246f8","attrs":{"85b81c0246f8":{"x":{},"y":{},"mode":"lines","alpha_stroke":1,"sizes":[10,100],"spans":[1,20],"type":"scatter"}},"layout":{"margin":{"b":40,"l":60,"t":25,"r":10},"xaxis":{"domain":[0,1],"automargin":true,"title":"x"},"yaxis":{"domain":[0,1],"automargin":true,"title":"random_y"},"hovermode":"closest","showlegend":false},"source":"A","config":{"modeBarButtonsToAdd":[{"name":"Collaborate","icon":{"width":1000,"ascent":500,"descent":-50,"path":"M487 375c7-10 9-23 5-36l-79-259c-3-12-11-23-22-31-11-8-22-12-35-12l-263 0c-15 0-29 5-43 15-13 10-23 23-28 37-5 13-5 25-1 37 0 0 0 3 1 7 1 5 1 8 1 11 0 2 0 4-1 6 0 3-1 5-1 6 1 2 2 4 3 6 1 2 2 4 4 6 2 3 4 5 5 7 5 7 9 16 13 26 4 10 7 19 9 26 0 2 0 5 0 9-1 4-1 6 0 8 0 2 2 5 4 8 3 3 5 5 5 7 4 6 8 15 12 26 4 11 7 19 7 26 1 1 0 4 0 9-1 4-1 7 0 8 1 2 3 5 6 8 4 4 6 6 6 7 4 5 8 13 13 24 4 11 7 20 7 28 1 1 0 4 0 7-1 3-1 6-1 7 0 2 1 4 3 6 1 1 3 4 5 6 2 3 3 5 5 6 1 2 3 5 4 9 2 3 3 7 5 10 1 3 2 6 4 10 2 4 4 7 6 9 2 3 4 5 7 7 3 2 7 3 11 3 3 0 8 0 13-1l0-1c7 2 12 2 14 2l218 0c14 0 25-5 32-16 8-10 10-23 6-37l-79-259c-7-22-13-37-20-43-7-7-19-10-37-10l-248 0c-5 0-9-2-11-5-2-3-2-7 0-12 4-13 18-20 41-20l264 0c5 0 10 2 16 5 5 3 8 6 10 11l85 282c2 5 2 10 2 17 7-3 13-7 17-13z m-304 0c-1-3-1-5 0-7 1-1 3-2 6-2l174 0c2 0 4 1 7 2 2 2 4 4 5 7l6 18c0 3 0 5-1 7-1 1-3 2-6 2l-173 0c-3 0-5-1-8-2-2-2-4-4-4-7z m-24-73c-1-3-1-5 0-7 2-2 3-2 6-2l174 0c2 0 5 0 7 2 3 2 4 4 5 7l6 18c1 2 0 5-1 6-1 2-3 3-5 3l-174 0c-3 0-5-1-7-3-3-1-4-4-5-6z"},"click":"function(gd) { \n        // is this being viewed in RStudio?\n        if (location.search == '?viewer_pane=1') {\n          alert('To learn about plotly for collaboration, visit:\\n https://cpsievert.github.io/plotly_book/plot-ly-for-collaboration.html');\n        } else {\n          window.open('https://cpsievert.github.io/plotly_book/plot-ly-for-collaboration.html', '_blank');\n        }\n      }"}],"cloud":false},"data":[{"x":[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,74,75,76,77,78,79,80,81,82,83,84,85,86,87,88,89,90,91,92,93,94,95,96,97,98,99,100],"y":[1.28634364183476,-0.021104090147719,1.07201412884853,1.81554344326637,-1.43044193484081,0.429101885760638,-1.05514817412152,2.71526084103711,0.60535097896408,-1.80974336884401,-0.279450748332269,-0.317159873479851,-2.00331362003447,-2.05569616836982,0.596557537994286,-0.697318047219005,-0.205852056936636,-1.36949879925729,0.054316373296536,-1.49274423174137,-0.503337821049463,-0.378735906603363,0.906058869136752,-0.064253498821835,-0.242831385515111,0.215849215863431,0.362934146164549,-0.417399739559007,0.591043085271599,-0.0521165359550275,-1.61091184897369,-1.50588086539131,0.506930564655416,-1.6602727371729,-0.463519524293679,0.89982829787332,-0.485698708262658,-0.36064996072437,0.0710410919438895,-0.534267592515747,0.721879586571838,-0.151873121569769,0.739562712403486,-0.673085327180735,0.1428153920087,0.931969377814236,-1.00887489670795,0.151718696978694,1.0173385547768,0.132803929963381,-1.63280340986758,-1.1019995349669,0.83654915654573,-1.10048277930905,2.30508023616576,0.189981612296513,-0.852475893616875,1.04097365279081,0.499773144652991,0.189465343492542,0.745909919963097,-0.0757706086835379,0.0200383744040778,-0.0194629789144172,-0.783445462640224,-0.336714466492315,0.402180529140958,1.12878541741476,0.160897035726177,-0.386524733277728,0.356228715386928,-1.21182372893312,-0.688432151162651,1.42875646421238,-0.912743321469973,0.638035148666747,-0.649386399194017,0.745955681179234,1.74900632752227,1.05895727743159,-0.4017618228572,-2.2141680837022,-1.72456964824067,-0.686937215717126,-0.363140349209708,-0.598332263539521,1.23798010005969,0.556295305841286,-1.01276919061498,0.638005375162059,-1.2717252532316,-0.372849357954387,-0.848167414810274,0.414510932565157,-0.192409129094314,-0.771027042211877,0.10350381275203,-1.56901622651936,1.38955776938163,-0.156239266195704],"mode":"lines","type":"scatter","marker":{"color":"rgba(31,119,180,1)","line":{"color":"rgba(31,119,180,1)"}},"error_y":{"color":"rgba(31,119,180,1)"},"error_x":{"color":"rgba(31,119,180,1)"},"line":{"color":"rgba(31,119,180,1)"},"xaxis":"x","yaxis":"y","frame":null}],"highlight":{"on":"plotly_click","persistent":false,"dynamic":false,"selectize":false,"opacityDim":0.2,"selected":{"opacity":1},"debounce":0},"base_url":"https://plot.ly"},"evals":["config.modeBarButtonsToAdd.0.click"],"jsHooks":[]}</script>

<!--/html_preserve-->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
