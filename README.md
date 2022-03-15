# wtf-workshop

<!-- badges: start -->
<!-- badges: end -->

This repo has two purposes:

  1. A place to record policies about how to run an instance of the "What They Forgot ..." (WTF) workshop, such as what to store where.
  1. Central storage for reusable assets that don't belong any where else, such as logos or diagrams.
  
Main types of content and where we store it:

  * [rstats.wtf](https://rstats.wtf) is a bookdown site where we aspire to
    develop a prose version of core WTF content, for wider availability and for
    workshop participants to consult afterwards. Source is here:
    <https://github.com/rstats-wtf/what-they-forgot>
  * Student-facing repo for each individual WTF offering, always billed as "The
    One True Location" the students need to bookmark and consult during the
    workshop. Might use GitHub Pages, might have an rstd.io shortlink. Has
    specifics about schedule, venue, WiFi, personnel. Contains links to
    everything else. Holds PDFs of slides. Examples:
    - rstudio::conf 2020 <https://github.com/rstats-wtf/wtf-2020-rsc>,
      uses GitHub Pages and a shortlink [rstd.io/wtf-2020-rsc](https://rstd.io/wtf-2020-rsc)
    - rstudio::conf 2019 <https://github.com/rstats-wtf/wtf-2019-rsc>,
      uses GitHub Pages and a shortlink [rstd.io/wtf-2019-rsc](https://rstd.io/wtf-2019-rsc)
    - Seattle October 2018 <https://github.com/rstats-wtf/wtf-2018-seattle>,
      uses a shortlink [rstd.io/wtf-seattle](https://rstd.io/wtf-seattle)
  * Individual activities used during the workshop. Typically downloaded by
    students using `usethis::use_course("rstats-wtf/REPO_NAME")` or
    `usethis::create_from_github("rstats-wtf/REPO_NAME")`. Examples:
    - <https://github.com/rstats-wtf/wtf-explore-libraries>
    - <https://github.com/rstats-wtf/wtf-debugging>
  * Completed versions of activities or a product created during live coding.
    Examples:
    - <https://github.com/rstats-wtf/wtf-packages-report-EXAMPLE>    
    - <https://github.com/rstats-wtf/wtf-live-intermediate-git-demo> *Jenny: I
      think I took a completed instance of `packages-report`, then used it as
      the Git repo to demo the intermediate/advanced Git workflows.*
  * Keynote slides. Stored in a shared instructors-only folder. We're currently
    testing a workflow using Google Drive. One subfolder for each "run" of WTF.
  * Reusable assets that don't change too rapidly belong here in this repo, even
    if the file format isn't terribly Git friendly. Examples: logos, icons,
    diagrams, ?Keynote templates?.
  
High-level guidance re: where to store a logical blob of content. When in doubt ...

  * Stick it in a public Git repo, within the rstats-wtf GitHub organization.
  * Try not to nest things.
    - Don't put a Git repo or RStudio Project inside another Git repo or RStudio
      Project.
    - Try not to put Git repos or RStudio Projects inside a cloud-syncing
      folder (such as on Google Drive or DropBox), because there are
      performance and privacy issues re: syncing of `.git/`, `.Rproj.user/`,
      `.Rhistory`, etc.
