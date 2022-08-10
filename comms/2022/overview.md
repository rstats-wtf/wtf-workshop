
## Overview

This is a two-day hands on workshop designed for experienced R and RStudio users who want to (re)design their R lifestyle.
You'll learn holistic workflows that address the most common sources of friction in data analysis.
We’ll work on project-oriented workflows, version control for data science (Git/GitHub!), maintaining your R installation, and how to plan for collaboration, communication, and iteration (incl. RMarkdown).

At the conclusion of the workshop, you should have: knowledge of your R installation that enhances your ability to maintain it, workflows that facilitate collaboration with yourself or others (including version control and strategies for file systems), tools to improve debugging processes, and methods to address repetitive tasks with the purrr package.

------------------------------------------------------------------------

## Is this course for me?

This course will be appropriate for you if you answer yes to these questions:

-   Have you been using R for a while and feel there might be better ways to organize your R life, but don't know what they are?

-   Do you want to streamline your workflow for doing analysis and automating repetitive tasks in R?

-   Are you willing to get into the weeds of your R installation, project organization, error messages, and source code?

------------------------------------------------------------------------

## Learning objectives

### Project-oriented workflow (2 sessions)

-   Establish the concept of the project as the basic organizational unit of work.
    RStudio offers rich support for this way of working via **P**rojects.

-   Describe benefits of project oriented workflows.

-   Apply best practices for working in RStudio projects, including

    -   Creating robust file paths that travel well in time and space (someone else's computer, your computer a year from now) with base R and with the {here} and {fs} packages.

    -   Constructing human and machine readable file names that sort nicely.

    -   Differentiating workflow elements, analysis inputs, and analysis outputs in project structure to create navigable programming interfaces.

    -   Restarting R frequently, with a blank slate.

### Git/GitHub (2 sessions)

-   Employ version control via git and GitHub with operations including commit, push and pull.

-   Fork and clone from remote repositories.

-   Describe importance of viewing commits and diffs.

-   Compile markdown reports from an R script for sharing code products on GitHub.

-   Create a project web site via GitHub Pages.

-   Compare and execute different methods to re-visit previous versions of projects.

-   Utilize branches as safety nets for code experimentation.

-   Explain situations that can create merge conflicts and strategies to resolve them.

### Personal R Administration (2 sessions)

-   Identify where software, packages, and configuration files are located on your operating system via base R, {fs}, {usethis}, and {devtools} functions.

-   Explain the scope and purpose of `.Renviron` and `.Rprofile` configuration files when starting R.
    Modify these files for your personal needs and preferences.

-   Employ strategies for package management, including establishing where packages are installed, how to upgrade and downgrade, how to install from source, and actual package managers.

-   Locate and navigate R package source code for better understanding of internal operations or troubleshooting.

-   Identify what is in your current R session (packages, versions); briefly introduce {renv} to create a reproducible environment.

### Debugging (1 session)

-   Locate and view function source code.

-   Examine function source code to generate insights on errors.

-   Apply strategies to effectively search GitHub.

-   Distinguish between strategies for debugging your own code versus someone else's code.

-   Discuss debugging functions (`traceback()`, `browser()`, `debug()`, `trace()`, and `recover()`) and the additional benefits of employing some of these strategies within RStudio.

### Iterating well with purrr (1 session)

-   Describe drawbacks of copying and pasting R code.

-   Complete tidyverse style code with the pipe operator (`%>%` in {magrittr}, and the newer `|>` in base R).

-   Accomplish iteration through vectorized functions.

-   Leverage `group_by()` as an iterative technique.

-   Explain differences between base R and {purrr} iterative functions.

-   Explore lists as an object to store information of varying types and sizes; explain how to extract elements from a list.

-   Apply functions from the `purrr::map_` family to perform iteration as an alternative to loops.
