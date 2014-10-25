---
title       : Guess My Iris!
subtitle    : A Client-facing App to Identify Irises
author      : Kyle Joecken
job         : Developing Data Products - Coursera
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Identification is Difficult!

### Can you tell the difference?

<img src="assets/img/three-irises.jpg">

### Can your clients?

--- .class #slide2

## Enter Guess My Iris!

### Take the guesswork out of plant identification.

1. Enter just a few simple measurements.

2. Let advanced algorithm detect faint data subtleties and return your species.



![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2.png) 

<ol start = "3">
      <li>Profit!</li>
</ol>

--- .class #slide3

## How It Works

Behind the scenes, a complex code emits a powerful prediction algorithm.


```r
fitMod <- train(Species ~ ., data = iris, method = "rpart")
fancyRpartPlot(fitMod$finalModel)
```

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3.png) 

--- .class #slide4

## Additional Features

- <b>Red herrings:</b> Sepal length and width entered but not used; this gives the
client an inflated sense of accuracy!

- <b>Sliders:</b> Easy to implement, slick, professional!

- <b>Built in documentation:</b> Even new gardeners and new computer users will find
it simple!

### Wish to try it yourself?

Give the app a test run [here](http://kielejocain.shinyapps.io/Project)!
