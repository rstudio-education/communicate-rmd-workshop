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

In this four-hour workshop, I will take you on a tour of how to get from
data to manuscript using R Markdown. Starting with a mock clinical trial
dataset, we’ll use R Markdown to combine prose, R code, and figures and
tables created with R code into a nicely formatted and reproducible
final manuscript.

We’ll work on template R Markdown documents from four different “phases”
of our mock clinical trial research project: an exploratory data
analysis, a progress report, a draft manuscript, and a final paper.
Along the way, we’ll learn about the basics of working with R Markdown
and how to include tables, data, and graphics.

## Learning objectives

Attendees will learn how to:

1.  Identify the basic anatomy of an R Markdown document. *(session 1)*

2.  Make and knit an R Markdown document. *(session 1)*

3.  Add text, R code, and output to an R Markdown document. *(session
    1)*

4.  Change the output format of an R Markdown document. *(session 2)*

5.  Use R code to create tables summarizing participants (i.e., a “Table
    One”) and statistical analyses within an R Markdown document.
    *(session 2)*

6.  Organize files and set up file paths when working in an R Markdown
    project. *(session 3)*

7.  Avoid growing pains as your R Markdown project evolves alongside
    your research project. *(session 3)*

8.  Export your figures and tables to a place you can find on your
    computer so you can share and re-use them. *(session 3)*

9.  Embed figures generated from R code in an R Markdown document,
    including multi-panel plots. *(session 4)*

10. Control how your figures look using `knitr` code chunk options,
    captions, and cross-references. *(session 4)*

11. Expand into new output formats like powerpoint presentations,
    conference posters, etc.- all built with R Markdown as the
    foundation *(wrap-up)*

## Is this course for me?

This introductory workshop is targeted at people who work in the medical
field who either don’t know or currently use R Markdown, or perhaps know
the basics but aren’t sure how R Markdown can fit into their research
workflow. No prior experience with R Markdown is required.

  - Have you written or collaborated on a medical manuscript to submit
    for publication to a peer-reviewed journal? Are you familiar with
    common components of a medical manuscript like a “Table One”, other
    summary tables, plots, text and citations?

  - Have you downloaded and used R a bit? Can you install and load
    packages?
    
      - *Even better,* have you used `tidyverse` packages like `ggplot2`
        and `dplyr`?

  - Have you used R with the RStudio Integrated Development Environment
    (IDE)? Are you familiar with the various “panes” and “tabs”? For
    instance, can you quickly find all objects in your current global
    environment, and can you send R code from a source file (.R, .Rmd)
    to the console?
    
      - *Even better,* have you tried to knit 🧶 an R Markdown document
        to some kind of output format like HTML, PDF, or Word?

## Instructor

Alison Hill is a Data Scientist & Professional Educator at RStudio.
Prior to joining RStudio, Dr. Hill was an Associate Professor and Center
Assistant Director at Oregon Health & Science University in Portland,
Oregon, where she was an NIH-funded Principal Investigator. Her
[work](https://profiles.impactstory.org/u/0000-0002-8082-1890) has been
published in
[Pediatrics](https://alison.rbind.io/publication/2015-obesity-in-asd-multisite/),
[Autism
Research](https://alison.rbind.io/publication/2016-uh-and-um-asd-sli/),
and [other peer-reviewed
journals](https://alison.rbind.io/publication/#2).

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
