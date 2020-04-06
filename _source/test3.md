---
title: "test 2"
output:
  md_document:
    variant: gfm
    preserve_yaml: TRUE
knit: (function(inputFile, encoding) {
   rmarkdown::render(inputFile, encoding = encoding, output_dir = "C:/Users/crist/Documents/GitHub/svmiller.github.io/_posts") })
author: "Cristian"
date: '2020-03-12'
excerpt: "Here is some R code contextualizing the Dow Jones' recent slide, because gallows humor is the only thing that keeps me warm at night."
layout: post
categories:
  - R
---



## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:


```r
summary(cars)
```

```
     speed           dist       
 Min.   : 4.0   Min.   :  2.00  
 1st Qu.:12.0   1st Qu.: 26.00  
 Median :15.0   Median : 36.00  
 Mean   :15.4   Mean   : 42.98  
 3rd Qu.:19.0   3rd Qu.: 56.00  
 Max.   :25.0   Max.   :120.00  
```

## Including Plots

You can also embed plots, for example:


```r
library(plotly)
library(htmlwidgets)
x <- c(1:100)
random_y <- rnorm(100, mean = 0)
data <- data.frame(x, random_y)

plot_ly(data, x = ~x, y = ~random_y, type = 'scatter', mode = 'lines')
```

```
Error in file(con, "rb"): no se puede abrir la conexión
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.


