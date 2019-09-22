R Markdown for Medicine: <br>From Data to Manuscript
================

### [R/Medicine 2019 conference](https://r-medicine.com/)

-----

<br>

:spiral\_calendar: September 30, 2019  
:clock8: 09:00am - 05:00pm  
:round\_pushpin: Canberra, Australia  
:white\_check\_mark: [Register](https://statsoc.org.au/event-3457232)  
:anchor:
[`ysc-rmarkdown.netlify.com`](https://ysc-rmarkdown.netlify.com/)

<br>

| Time          | Activity                        |
| :------------ | :------------------------------ |
| 09:00 - 10:30 | Session 1 (R Markdown Basics)   |
| 10:30 - 11:00 | *Break* :tea:                   |
| 11:00 - 12:30 | Session 2 (Advanced R Markdown) |
| 12:30 - 01:30 | *Lunch* :bento:                 |
| 01:30 - 03:00 | Session 3 (Templates)           |
| 03:00 - 03:30 | *Break* :tea:                   |
| 03:30 - 05:00 | Session 4 (Collections)         |

<br>

<!--
01
-use ozbabynames/usbabynames
-make parameterized rmd with plots (added more on params here)
-> deploy at end!

02- focus on HTML outputs [cut version control]
-knit to bookdown (not just for books!) ?
-knit to distill (not just for ML!) ?
-maybe add in generations here
? where to include oz bakeoff?
-knit to flexdashboard
-knit to xaringan
-maybe include good HTML widgets like leaflet for mapping

Where to go?
-knit from the command line
-knitting parameterized reports from the command line

03- templates inside a package
-build an opinionated template with custom things in it
-data?
-->

-----

## Overview

In this full-day workshop, you’ll learn how to get more out of R
Markdown (and friends). We will demystify how R Markdown works under the
hood. You will learn practical tools and workflows to increase your
efficiency and productivity using R Markdown (including RStudio IDE
features and templates), while learning how to use some extension
packages along the way. We assume that you have knit an R Markdown
document before, but you don’t need to be an advanced R Markdown user to
take this workshop.

## Instructor

Alison Hill is a Data Scientist & Professional Educator at RStudio. She
received her PhD in psychology and quantitative methods from Vanderbilt
University in 2008. Prior to joining RStudio, she was an Assistant
Professor at Arizona State University, and an Associate Professor at
Oregon Health & Science University (OHSU). Alison is one of the keynote
speakers at the 2019 Young Statisticians Conference. She regularly leads
workshops and develops online learning materials on topics like
reproducible research, machine learning, and data visualization. She is
also a co-author of the book ‘blogdown: Creating Websites with R
Markdown’ (<https://bookdown.org/yihui/blogdown/>). Alison lives in
Portland, Oregon with her husband and young daughter.

## Pre-work

Welcome to the [Communicating with R Markdown](/) workshop\! We look
forward to meeting you in person. Before attending the workshop, please
complete the following prework:

1.  Sign up for a free RStudio Cloud account at <https://rstudio.cloud/>
    before the workshop. I recommend logging in with an existing Google
    or GitHub account, if you have one (rather than creating a new
    account with another password you have to remember).

2.  We will be using GitHub in this workshop for version control and
    publishing. Sign up for a free GitHub.com account at
    <https://github.com/join> if you don’t already have one. Also:
    
      - Complete these [installation
        instructions](https://happygitwithr.com/install-intro.html).
    
      - Test your connection between GitHub and RStudio following [these
        steps](https://happygitwithr.com/connect-intro.html).
    
      - **NOTE:** We *strongly recommend* that if you are not already a
        fluent GitHub user you choose [HTTPS over
        SSH](https://happygitwithr.com/credential-caching.html).

3.  Complete this [10-minute interactive tutorial on
    Markdown](https://commonmark.org/help/tutorial/).

4.  Please bring a laptop that has the following installed:
    
      - A recent version of R (\>=3.6.0), which is available for free at
        <https://cloud.r-project.org/>
    
      - A recent version of RStudio Desktop (\>=1.2), available for free
        ([RStudio Desktop Open Source
        License](https://www.rstudio.com/products/rstudio/download/#download))
    
      - The R packages we will use, which you can install by connecting
        to the internet, opening RStudio, and running at the command
        line:
        
        ``` r
        install.packages(c("rmarkdown", "devtools", "usethis", "here", 
                           "tidyverse", "xaringan", "flexdashboard", 
                           "distill", "bookdown", "blogdown"))
        ```

5.  Don’t forget your power cord\!

On the day of the workshop, I’ll provide you with an RStudio Cloud
project that contains all of the course materials. We will use the
software listed above only as an important backup should there be
problems with the on-site internet connection.

[View slides](/slides/00-loop.html) *(note: these slides are
intentionally a loop and will play on
autoadvance)*

-----

[![forthebadge](https://forthebadge.com/images/badges/cc-by.svg)](https://creativecommons.org/licenses/by/4.0/)  
This work is licensed under a [Creative Commons Attribution 4.0
International License](https://creativecommons.org/licenses/by/4.0/).
