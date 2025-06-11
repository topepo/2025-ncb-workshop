Making Project Work Better with R 
================

### 9th Biennial Nonclinical Biostatistics Conference

by Max Kuhn + E. David Aja 

-----

:spiral_calendar: June 16, 2025  
:alarm_clock:     08:30 - 12:00  
:hotel:           Room A 
:writing_hand:    [github.com/topepo/2025-ncb-workshop](https://github.com/topepo/2025-ncb-workshop)

-----

# Description

> I need to make sure that my future self isn’t going to be mad at my present self. - Kjell Johnson

A nonclinical statistician often has many simultaneous data analysis projects. Some of these may have been handed to them and others might eventually be handed to someone else. What are good practices for organizing and maintaining the raw data, source files, results, and other artifacts when doing data analysis?

We’ll discuss some tools to

- Understanding project-oriented workflows
- Organize your project work
- Painlessly write good R code
- Manage changes to code and data
- Write resilient project reports
- Enable reproducibility

# Audience

Participants should have some experience with R, Rmarkdown/Quarto, and have used the RStudio IDE.

## Prework

1. Please have two recent versions of R installed (say >= 4.4), as well as a recent version of [RStudio](https://posit.co/download/rstudio-desktop/). 

You can find older versions of R [at this link for Windows](https://cran.r-project.org/bin/windows/base/old/) (click on the `.exe` file to install), at [this link for Intel Macs](https://cran.r-project.org/bin/macosx/big-sur-x86_64/base/), and at [this link for M-series Macs.](https://cran.r-project.org/bin/macosx/big-sur-arm64/base/)

See the discussion in Install or upgrade R and RStudio: https://happygitwithr.com/install-r-rstudio.html#install-r-rstudio

2. Install packages

```r
install.packages("pak")
library(pak)

pkgs <- c("cli", "devtools", "epoxy", "fs", "glue", "gtExtras", "gtsummary", "hadley/emo", 
          "here", "prettyunits", "renv", "rmarkdown", "tidyverse", "usethis", "xfun")
pak(pkgs)
```

3. Please make sure your system is ready to build packages. You can  confirm this by checking if `devtools::has_devel()` returns `Your system is ready to build packages!`.  If this returns `Could not find tools necessary to compile a package` this indicates your system needs additional tools - please see https://rstats-wtf.github.io/wtf-personal-radmin-slides/#/how-to-get-the-tools to identify what to install for your OS.

## Schedule

| Time          | Activity                                        | Instructor      |
|:--------------|:------------------------------------------------|:----------------|
| 08:30          | Workshop Begins                                | Max and David   |
| 09:30 - 10:00  | *Bio Break*                                    |                 |
| 12:00          | Workshop Ends                                  | Max and David   |

## Instructor(s)

[Max Kuhn](https://max-kuhn.org/) is a statistician working at Posit PBC, formerly of Pfizer R&D (Discovery) and BD (molecular diagnostics).

[E. David Aja](https://edavidaja.com/) is a Solutions Engineer at Posit. Before joining Posit, he worked as a data scientist in the public sector.

-----

![](https://i.creativecommons.org/l/by/4.0/88x31.png) This work is
licensed under a [Creative Commons Attribution 4.0 International
License](https://creativecommons.org/licenses/by/4.0/).
