---
title: "Installing R and easystats"
author: "Dominique Makowski"
author_web: https://dominiquemakowski.github.io/
date: 2019-02-21
categories: ["R", "easystats"]
tags: ["installation", "easystats"]
summary: This post shows how to quickly install R, R studio and the eaystats packages.
---


## Install R and R Studio

-   Go here: <https://cloud.r-project.org/>
-   Download the last version for your OS
-   Install it
-   Go here: <https://www.rstudio.com/products/rstudio/download/#download>
-   Download the right version for your OS
-   Install it
-   Start R studio

## Install the easystats packages

The easystats packages can be installed at once. If you wish to do so, enter one of the following in the console and press enter:

```r
install.packages("devtools")
library(devtools)
devtools::install_github("easystats/easystats")
```

Once the packages are installed, you can load them all by putting the following at the beginning of every script:

```r
library(easystats)
```