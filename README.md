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
    everything else. Holds PDFs of slides. 
    
    The conf workshop coordinators often like to have one central organisation
    for these repos. I do not like this because I don't want the content for
    individual instances of WTF to spread out over various GitHub orgs which I
    do not have admin privileges on.
    
    Compromise: we comply with whatever the coordinators ask us to do. But we
    also always make sure that the the definitive copy of the materials is here
    in the rstats-wtf org, at least in the long run.

    - rstudio::conf 2022 <https://github.com/rstats-wtf/wtf-2022-rsc>
      
      Example of the conf-owned type of repo the coordinators want us to use:
      <https://github.com/rstudio-conf-2022/wtf-rstats>
      
    - rstudio::conf 2020 <https://github.com/rstats-wtf/wtf-2020-rsc>,
      uses GitHub Pages and a shortlink [rstd.io/wtf-2020-rsc](https://rstd.io/wtf-2020-rsc)
      
      Note in the README: This repo previously belonged to the GitHub
      organization <https://github.com/rstudio-conf-2020>, under the name
      `what-they-forgot`. It was renamed and transferred here, as preparations
      for rstudio::conf(2022) started. It is useful to us to keep all of our
      resources within one persistent organization.
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
  * Keynote slides. Stored in a shared instructors-only folder on Google Drive,
    owned by Jenny. One subfolder for each "run" of WTF (or for any event where
    some portion of the materials are presented).
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

### Notes

There used to be a `git-diagrams` folder here, but I've removed it because it was confusing.
The most current Git images used in WTF slides about Git/GitHub are maintained within the Happy Git space.

### Additional assets

* keynote slides for git/github section are on Jenny's [google drive](https://drive.google.com/drive/u/0/folders/1Qht4U8lIPoQMkNLoyQy-gMidvICsesQq)

* intro / outro decks for 2022 rstudio conf are on Shannon's google slides [opening](https://docs.google.com/presentation/d/1JNWIDMG7G8inZQ66uXOaUAEBoENgF0MTwEHdRDSpn6M/edit?usp=sharing), [closing](https://docs.google.com/presentation/d/1NojVP3lZk84WYA0ZemDWjFHxwL3mKL-xrY6f9RWzNJI/edit?usp=sharing)



