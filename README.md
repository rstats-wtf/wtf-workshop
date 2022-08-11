# wtf-workshop

This repo has two purposes:

1.  A place to record policies about how to run an instance of the "What They Forgot ..." (WTF) workshop, such as what to store where.
2.  Central storage for reusable assets that don't belong any where else, such as logos or diagrams.

Main types of content and where we store it:

-   [rstats.wtf](https://rstats.wtf) is a bookdown site where we aspire to develop a prose version of core WTF content, for wider availability and for workshop participants to consult afterwards.
    Source is here: <https://github.com/rstats-wtf/what-they-forgot>

-   Student-facing repo for each individual WTF offering, always billed as "The One True Location" the students need to bookmark and consult during the workshop.
    Might use GitHub Pages, might have an rstd.io shortlink.
    Has specifics about schedule, venue, WiFi, personnel.
    Contains links to everything else.
    Holds PDFs of slides.

    The conf workshop coordinators often like to have one central organisation for these repos.
    I do not like this because I don't want the content for individual instances of WTF to spread out over various GitHub orgs which I do not have admin privileges on.

    Compromise: we comply with whatever the coordinators ask us to do.
    But we also always make sure that the the definitive copy of the materials is here in the rstats-wtf org, at least in the long run.

    -   rstudio::conf 2022 <https://github.com/rstats-wtf/wtf-2022-rsc>

        Example of the conf-owned type of repo the coordinators want us to use: <https://github.com/rstudio-conf-2022/wtf-rstats>

        Repos were dually maintained via [pushing content to two remotes](https://stackoverflow.com/questions/14290113/git-pushing-code-to-two-remotes/14290145#14290145)

    -   rstudio::conf 2020 <https://github.com/rstats-wtf/wtf-2020-rsc>, uses GitHub Pages and a shortlink [rstd.io/wtf-2020-rsc](https://rstd.io/wtf-2020-rsc)

        Note in the README: This repo previously belonged to the GitHub organization <https://github.com/rstudio-conf-2020>, under the name `what-they-forgot`.
        It was renamed and transferred here, as preparations for rstudio::conf(2022) started.
        It is useful to us to keep all of our resources within one persistent organization.

    -   rstudio::conf 2019 <https://github.com/rstats-wtf/wtf-2019-rsc>, uses GitHub Pages and a shortlink [rstd.io/wtf-2019-rsc](https://rstd.io/wtf-2019-rsc)

    -   Seattle October 2018 <https://github.com/rstats-wtf/wtf-2018-seattle>, uses a shortlink [rstd.io/wtf-seattle](https://rstd.io/wtf-seattle)

-   Individual activities used during the workshop.
    Typically downloaded by students using `usethis::use_course("rstats-wtf/REPO_NAME")` or `usethis::create_from_github("rstats-wtf/REPO_NAME")`.
    Examples:

    -   <https://github.com/rstats-wtf/wtf-explore-libraries>
    -   <https://github.com/rstats-wtf/wtf-debugging>

-   Completed versions of activities or a product created during live coding.
    Examples:

    -   <https://github.com/rstats-wtf/wtf-packages-report-EXAMPLE>\
    -   <https://github.com/rstats-wtf/wtf-live-intermediate-git-demo> *Jenny: I think I took a completed instance of `packages-report`, then used it as the Git repo to demo the intermediate/advanced Git workflows.*

-   Keynote slides.
    Stored in a shared instructors-only folder on Google Drive, owned by Jenny.
    One subfolder for each "run" of WTF (or for any event where some portion of the materials are presented).

-   Reusable assets that don't change too rapidly belong here in this repo, even if the file format isn't terribly Git friendly.
    Examples: logos, icons, diagrams, ?K
    eynote templates?.

High-level guidance re: where to store a logical blob of content.
When in doubt ...

-   Stick it in a public Git repo, within the rstats-wtf GitHub organization.
-   Try not to nest things.
    -   Don't put a Git repo or RStudio Project inside another Git repo or RStudio Project.
    -   Try not to put Git repos or RStudio Projects inside a cloud-syncing folder (such as on Google Drive or DropBox), because there are performance and privacy issues re: syncing of `.git/`, `.Rproj.user/`, `.Rhistory`, etc.

### Notes

There used to be a `git-diagrams` folder here, but I've removed it because it was confusing.
The most current Git images used in WTF slides about Git/GitHub are maintained within the Happy Git space.

# 2022 RStudio Conference


| Content                   | Slide type    | Slide source                                                                                               | Exercises                                                                                                                                                                                                            |
|---------------|---------------|---------------|----------------------------|
| Intro slides              | google slides | [drive assests](https://drive.google.com/drive/u/0/folders/12shxFDi5SPjwS6vc8UVIJRJZOQoeViV9)              | In slides (place emoji on issue to ensure logged in)                                                                                                                                                                 |
| Project oriented workflow | quarto        | [wtf-project-oriented-workflow-slides](https://github.com/rstats-wtf/wtf-project-oriented-workflow-slides) | [wtf-explore-libraries](https://github.com/rstats-wtf/wtf-explore-libraries), [wtf-fix-paths](https://github.com/rstats-wtf/wtf-fix-paths), [wtf-packages-report](https://github.com/rstats-wtf/wtf-packages-report) |
| Debugging                 | quarto        | [wtf-debugging-slides](https://github.com/rstats-wtf/wtf-debugging-slides)                                 | [wtf-debugging](https://github.com/rstats-wtf/wtf-debugging), associated pkg [wtfdbg](https://github.com/rstats-wtf/wtfdbg)                                                                                          |
| Git/GitHub                | keynote       | [drive assests](https://drive.google.com/drive/u/0/folders/12shxFDi5SPjwS6vc8UVIJRJZOQoeViV9)              | In slides                                                                                                                                                                                                            |
| Personal R Administration | quarto        | [wtf-personal-radmin-slides](https://github.com/rstats-wtf/wtf-personal-radmin-slides)                     | In slides                                                                                                                                                                                                            |
| Iterating well with purrr | quarto        | [wtf-purrr-slides](https://github.com/rstats-wtf/wtf-purrr-slides)                                         | In slides                                                                                                                                                                                                            |
| Closing slides            | google slides | [drive assests](https://drive.google.com/drive/u/0/folders/12shxFDi5SPjwS6vc8UVIJRJZOQoeViV9)              | None                                                                                                                                                                                                                 |





+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| Content                   | Slide         | Slide                                                                                                      | Slides                                                                                                               | Exercises                                                                    |
|                           |               |                                                                                                            |                                                                                                                      |                                                                              |
|                           | type          | source                                                                                                     | rendered                                                                                                             |                                                                              |
+===========================+===============+============================================================================================================+======================================================================================================================+==============================================================================+
| Intro slides              | google slides | [drive assests](https://drive.google.com/drive/u/0/folders/12shxFDi5SPjwS6vc8UVIJRJZOQoeViV9)              | [materials](https://github.com/rstats-wtf/wtf-2022-rsc/blob/main/materials/wtf-opening-2022.pdf)                     | In slides (place emoji on issue to ensure logged in)                         |
+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| Project oriented workflow | quarto        | [wtf-project-oriented-workflow-slides](https://github.com/rstats-wtf/wtf-project-oriented-workflow-slides) | [ghpages](https://rstats-wtf.github.io/wtf-project-oriented-workflow-slides/#/title-slide)                           | [wtf-explore-libraries](https://github.com/rstats-wtf/wtf-explore-libraries) |
|                           |               |                                                                                                            |                                                                                                                      |                                                                              |
|                           |               |                                                                                                            |                                                                                                                      | [wtf-fix-paths](https://github.com/rstats-wtf/wtf-fix-paths)                 |
|                           |               |                                                                                                            |                                                                                                                      |                                                                              |
|                           |               |                                                                                                            |                                                                                                                      | [wtf-packages-report](https://github.com/rstats-wtf/wtf-packages-report)     |
+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| Debugging                 | quarto        | [wtf-debugging-slides](https://github.com/rstats-wtf/wtf-debugging-slides)                                 | [ghpages](https://rstats-wtf.github.io/wtf-debugging-slides/#/title-slide)                                           | [wtf-debugging](https://github.com/rstats-wtf/wtf-debugging)                 |
|                           |               |                                                                                                            |                                                                                                                      |                                                                              |
|                           |               |                                                                                                            |                                                                                                                      | associated pkg [wtfdbg](https://github.com/rstats-wtf/wtfdbg)                |
+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| Git/GitHub                | keynote       | [drive assests](https://drive.google.com/drive/u/0/folders/12shxFDi5SPjwS6vc8UVIJRJZOQoeViV9)              | [daily-workflows](https://github.com/rstats-wtf/wtf-2022-rsc/blob/main/materials/git-and-github-daily-workflows.pdf) | In slides                                                                    |
|                           |               |                                                                                                            |                                                                                                                      |                                                                              |
|                           |               |                                                                                                            | [early-usage](https://github.com/rstats-wtf/wtf-2022-rsc/blob/main/materials/git-and-github-early-usage.pdf)         |                                                                              |
+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| Personal R Administration | quarto        | [wtf-personal-radmin-slides](https://github.com/rstats-wtf/wtf-personal-radmin-slides)                     | [ghpages](https://rstats-wtf.github.io/wtf-personal-radmin-slides/#/personal-r-administration)                       | In slides                                                                    |
+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| Iterating well with purrr | quarto        | [wtf-purrr-slides](https://github.com/rstats-wtf/wtf-purrr-slides)                                         | [ghpages](https://rstats-wtf.github.io/wtf-purrr-slides/#/title-slide)                                               | In slides                                                                    |
+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+
| Closing slides            | google slides | [drive assests](https://drive.google.com/drive/u/0/folders/12shxFDi5SPjwS6vc8UVIJRJZOQoeViV9)              | [materials](https://github.com/rstats-wtf/wtf-2022-rsc/blob/main/materials/wtf-closing-2022.pdf)                     | None                                                                         |
+---------------------------+---------------+------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+------------------------------------------------------------------------------+

-   drive assets are private, ask Jenny for access to materials
-   keynote and google slide rendered pdfs are available in workshop repos `/materials`
