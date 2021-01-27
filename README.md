Lab 2: Introduction to RStudio
================
SIMEON ALFA
2021-01-27

Welcome to my Lab 2 repository for Quantitative Biology BIOL 275 at
MSUM.

## Lab objectives

The objectives of this lab are:

-   Use the console and source windows in RStudio
-   Write and run code in an R script
-   Document your R code with comments
-   Transfer code from an R script to an R Markdown document
-   Craft a narrative combining text explanation, code, and graphs
-   Collaborate on Issues in GitHub
-   Conduct peer review of an assignment

## Repository contents

The repository contains the following scripts:

-   [calculator.R](calculator.R)
-   [Lab 2 assignment](assignment_lab-2.md)

## Instructions for knitting

Your actual README document must be a Markdown file. This one is an R
Markdown file.

When you are done editing this document, click the Knit button in the
Source Pane. RStudio will then convert this into a .md file and give you
a preview in a separate window. Make sure everything looks okay and then
close the preview window.

## R Markdown

This README is an R Markdown document (.Rmd), which means you can use
markdown syntax and you can embed code chunks.

Here is a list of resources for helping you write R Markdown documents:

-   In the Go to the **Help** menu and select **Markdown Quick
    Reference**
-   [Basic Syntax](https://www.markdownguide.org/basic-syntax/) on the
    Markdown Guide website

## Session Info

Here is my session information:

``` r
sessioninfo::session_info(c("tidyverse"))
```

    ## - Session info ---------------------------------------------------------------
    ##  setting  value                       
    ##  version  R version 4.0.3 (2020-10-10)
    ##  os       Windows 10 x64              
    ##  system   x86_64, mingw32             
    ##  ui       RTerm                       
    ##  language (EN)                        
    ##  collate  English_United States.1252  
    ##  ctype    English_United States.1252  
    ##  tz       America/Chicago             
    ##  date     2021-01-27                  
    ## 
    ## - Packages -------------------------------------------------------------------
    ##  package      * version  date       lib source        
    ##  askpass        1.1      2019-01-13 [1] CRAN (R 4.0.3)
    ##  assertthat     0.2.1    2019-03-21 [1] CRAN (R 4.0.3)
    ##  backports      1.2.0    2020-11-02 [1] CRAN (R 4.0.3)
    ##  base64enc      0.1-3    2015-07-28 [1] CRAN (R 4.0.3)
    ##  BH             1.75.0-0 2021-01-11 [1] CRAN (R 4.0.3)
    ##  blob           1.2.1    2020-01-20 [1] CRAN (R 4.0.3)
    ##  brio           1.1.0    2020-08-31 [1] CRAN (R 4.0.3)
    ##  broom          0.7.3    2020-12-16 [1] CRAN (R 4.0.3)
    ##  callr          3.5.1    2020-10-13 [1] CRAN (R 4.0.3)
    ##  cellranger     1.1.0    2016-07-27 [1] CRAN (R 4.0.3)
    ##  cli            2.2.0    2020-11-20 [1] CRAN (R 4.0.3)
    ##  clipr          0.7.1    2020-10-08 [1] CRAN (R 4.0.3)
    ##  colorspace     2.0-0    2020-11-11 [1] CRAN (R 4.0.3)
    ##  cpp11          0.2.5    2021-01-12 [1] CRAN (R 4.0.3)
    ##  crayon         1.3.4    2017-09-16 [1] CRAN (R 4.0.3)
    ##  curl           4.3      2019-12-02 [1] CRAN (R 4.0.3)
    ##  DBI            1.1.1    2021-01-15 [1] CRAN (R 4.0.3)
    ##  dbplyr         2.0.0    2020-11-03 [1] CRAN (R 4.0.3)
    ##  desc           1.2.0    2018-05-01 [1] CRAN (R 4.0.3)
    ##  diffobj        0.3.3    2021-01-07 [1] CRAN (R 4.0.3)
    ##  digest         0.6.27   2020-10-24 [1] CRAN (R 4.0.3)
    ##  dplyr          1.0.3    2021-01-15 [1] CRAN (R 4.0.3)
    ##  ellipsis       0.3.1    2020-05-15 [1] CRAN (R 4.0.3)
    ##  evaluate       0.14     2019-05-28 [1] CRAN (R 4.0.3)
    ##  fansi          0.4.2    2021-01-15 [1] CRAN (R 4.0.3)
    ##  farver         2.0.3    2020-01-16 [1] CRAN (R 4.0.3)
    ##  forcats        0.5.0    2020-03-01 [1] CRAN (R 4.0.3)
    ##  fs             1.5.0    2020-07-31 [1] CRAN (R 4.0.3)
    ##  generics       0.1.0    2020-10-31 [1] CRAN (R 4.0.3)
    ##  ggplot2        3.3.3    2020-12-30 [1] CRAN (R 4.0.3)
    ##  glue           1.4.2    2020-08-27 [1] CRAN (R 4.0.3)
    ##  gtable         0.3.0    2019-03-25 [1] CRAN (R 4.0.3)
    ##  haven          2.3.1    2020-06-01 [1] CRAN (R 4.0.3)
    ##  highr          0.8      2019-03-20 [1] CRAN (R 4.0.3)
    ##  hms            1.0.0    2021-01-13 [1] CRAN (R 4.0.3)
    ##  htmltools      0.5.0    2020-06-16 [1] CRAN (R 4.0.3)
    ##  httr           1.4.2    2020-07-20 [1] CRAN (R 4.0.3)
    ##  isoband        0.2.3    2020-12-01 [1] CRAN (R 4.0.3)
    ##  jsonlite       1.7.2    2020-12-09 [1] CRAN (R 4.0.3)
    ##  knitr          1.30     2020-09-22 [1] CRAN (R 4.0.3)
    ##  labeling       0.4.2    2020-10-20 [1] CRAN (R 4.0.3)
    ##  lattice        0.20-41  2020-04-02 [2] CRAN (R 4.0.3)
    ##  lifecycle      0.2.0    2020-03-06 [1] CRAN (R 4.0.3)
    ##  lubridate      1.7.9.2  2020-11-13 [1] CRAN (R 4.0.3)
    ##  magrittr       2.0.1    2020-11-17 [1] CRAN (R 4.0.3)
    ##  markdown       1.1      2019-08-07 [1] CRAN (R 4.0.3)
    ##  MASS           7.3-53   2020-09-09 [2] CRAN (R 4.0.3)
    ##  Matrix         1.2-18   2019-11-27 [2] CRAN (R 4.0.3)
    ##  mgcv           1.8-33   2020-08-27 [2] CRAN (R 4.0.3)
    ##  mime           0.9      2020-02-04 [1] CRAN (R 4.0.3)
    ##  modelr         0.1.8    2020-05-19 [1] CRAN (R 4.0.3)
    ##  munsell        0.5.0    2018-06-12 [1] CRAN (R 4.0.3)
    ##  nlme           3.1-149  2020-08-23 [2] CRAN (R 4.0.3)
    ##  openssl        1.4.3    2020-09-18 [1] CRAN (R 4.0.3)
    ##  pillar         1.4.7    2020-11-20 [1] CRAN (R 4.0.3)
    ##  pkgbuild       1.2.0    2020-12-15 [1] CRAN (R 4.0.3)
    ##  pkgconfig      2.0.3    2019-09-22 [1] CRAN (R 4.0.3)
    ##  pkgload        1.1.0    2020-05-29 [1] CRAN (R 4.0.3)
    ##  praise         1.0.0    2015-08-11 [1] CRAN (R 4.0.3)
    ##  prettyunits    1.1.1    2020-01-24 [1] CRAN (R 4.0.3)
    ##  processx       3.4.5    2020-11-30 [1] CRAN (R 4.0.3)
    ##  progress       1.2.2    2019-05-16 [1] CRAN (R 4.0.3)
    ##  ps             1.5.0    2020-12-05 [1] CRAN (R 4.0.3)
    ##  purrr          0.3.4    2020-04-17 [1] CRAN (R 4.0.3)
    ##  R6             2.5.0    2020-10-28 [1] CRAN (R 4.0.3)
    ##  RColorBrewer   1.1-2    2014-12-07 [1] CRAN (R 4.0.3)
    ##  Rcpp           1.0.5    2020-07-06 [1] CRAN (R 4.0.3)
    ##  readr          1.4.0    2020-10-05 [1] CRAN (R 4.0.3)
    ##  readxl         1.3.1    2019-03-13 [1] CRAN (R 4.0.3)
    ##  rematch        1.0.1    2016-04-21 [1] CRAN (R 4.0.3)
    ##  rematch2       2.1.2    2020-05-01 [1] CRAN (R 4.0.3)
    ##  reprex         0.3.0    2019-05-16 [1] CRAN (R 4.0.3)
    ##  rlang          0.4.10   2020-12-30 [1] CRAN (R 4.0.3)
    ##  rmarkdown      2.6      2020-12-14 [1] CRAN (R 4.0.3)
    ##  rprojroot      2.0.2    2020-11-15 [1] CRAN (R 4.0.3)
    ##  rstudioapi     0.13     2020-11-12 [1] CRAN (R 4.0.3)
    ##  rvest          0.3.6    2020-07-25 [1] CRAN (R 4.0.3)
    ##  scales         1.1.1    2020-05-11 [1] CRAN (R 4.0.3)
    ##  selectr        0.4-2    2019-11-20 [1] CRAN (R 4.0.3)
    ##  stringi        1.5.3    2020-09-09 [1] CRAN (R 4.0.3)
    ##  stringr        1.4.0    2019-02-10 [1] CRAN (R 4.0.3)
    ##  sys            3.4      2020-07-23 [1] CRAN (R 4.0.3)
    ##  testthat       3.0.1    2020-12-17 [1] CRAN (R 4.0.3)
    ##  tibble         3.0.5    2021-01-15 [1] CRAN (R 4.0.3)
    ##  tidyr          1.1.2    2020-08-27 [1] CRAN (R 4.0.3)
    ##  tidyselect     1.1.0    2020-05-11 [1] CRAN (R 4.0.3)
    ##  tidyverse      1.3.0    2019-11-21 [1] CRAN (R 4.0.3)
    ##  tinytex        0.28     2020-12-14 [1] CRAN (R 4.0.3)
    ##  utf8           1.1.4    2018-05-24 [1] CRAN (R 4.0.3)
    ##  vctrs          0.3.6    2020-12-17 [1] CRAN (R 4.0.3)
    ##  viridisLite    0.3.0    2018-02-01 [1] CRAN (R 4.0.3)
    ##  waldo          0.2.3    2020-11-09 [1] CRAN (R 4.0.3)
    ##  whisker        0.4      2019-08-28 [1] CRAN (R 4.0.3)
    ##  withr          2.4.0    2021-01-16 [1] CRAN (R 4.0.3)
    ##  xfun           0.20     2021-01-06 [1] CRAN (R 4.0.3)
    ##  xml2           1.3.2    2020-04-23 [1] CRAN (R 4.0.3)
    ##  yaml           2.2.1    2020-02-01 [1] CRAN (R 4.0.3)
    ## 
    ## [1] C:/Users/simeo/Documents/R/win-library/4.0
    ## [2] C:/Program Files/R/R-4.0.3/library
