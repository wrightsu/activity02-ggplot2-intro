Activity 2 - `{ggplot2}` intro
================

It is assumed that you have read Sections 3.1–3.4 of R4DS and completed
Preparation 3 prior to completing this activity.

In this activity, you will:

-   Create boxplots and scatterplot visualizations using `{ggplot2}`.
-   Combine multiple geometric layers in one visualization.
-   Identify when to map an aesthetic to a feature of a dataset or set
    to a specific value.

## ☑️ Task 1: The Workflow

Remember to take these steps slowly, help each other out, and get a hold
of your instructor when you have questions or issues. These directions
have been slightly modified from Activity 1 to hopefully further reduce
these steps in Activity 3.1 and beyond.

**You may need your PAT that you created in Preparation 2**. If you
misplaced this token, you will need to create a new one prior to
beginning these steps.

1.  In this GitHub repo, click on the ![fork](README-img/fork-icon.png)
    **Fork** icon near the upper-right-hand corner. You should be taken
    a copy of this repo that is in your GitHub account - your page title
    should be `{username}/activity02-ggplot2-intro`, where `{username}`
    is replaced with your GitHub username.
2.  Click on the green **Code** button.

-   Verify that the drop-down identifies that you are using the
    **HTTPS** method (this is *probably* the default view; otherwise,
    select “HTTPS”).
-   Click on the ![clipboard](README-img/clipboard-icon.png) icon to
    copy the repo HTTPS information.

3.  Log in to the [RStudio Server](https://rstudio.gvsu.edu/).

-   Verify that you are in an RStudio session (it doesn’t matter if it
    is a previous Project session or a “vanilla” RStudio session).

4.  **ONE TIME ONLY** Note that we are using Git syntax to (hopefully)
    store your GitHub credentials in RStudio for the entire semester
    (for ten millions seconds or just over 16 weeks).
    -   In the **Console** pane (left-hand pane), select the
        **Terminal** tab. Once this loads, you should see a line of
        information followed by a `$` and blinking cursor. Here, type
        the following and press Enter/Return (note the use of single
        quotation marks):

    ``` bash
    git config --global credential.helper 'cache -timeout=10000000'
    ```
5.  Create a new Project. You can do this by clicking on the
    <img src="README-img/new-project-icon.png" alt="new project" width = "20"/>
    icon or through the menus (File &gt; New Project…).

-   In the *New Project Wizard* pop-up, select **Version Control** on
    the *Create Project* screen, then select **Git** on the *Create
    Project from Version Control* screen.
-   On the *Clone Git Repository* screen, paste the HTTPS information
    from (2) into the *Repository URL* dialog box. It should look like:
    `https://github.com/<username>/activity02-ggplot2-intro.git`
-   The *Project directory name* dialog box should automatically
    populate with your repository name, but sometimes Macs have an issue
    with this (if so, click into this box and press the ![command
    key](README-img/command-key-icon.png) command key on your keyboard).
    It should look something like: `activity02-ggplot2-intro`
-   In the *Create project as subdirectory of* dialog box, click on
    **Browse**.
-   In the *Choose Directory* pop-up, navigate to your class-level
    folder (i.e., you were encouraged to create a folder named either
    `STA418` or `STA518`) You were also encouraged to create
    an`activities` folder within your class-level folder to help
    organize our materials. Once you have navigated to the folder you
    wish this repo to be located, click **Choose**.
-   Verify that the *Create project as a directory of* dialog box
    contains the folder location that you previously specified, then
    click on **Create Project**.
-   You may be asked to login with your GitHub credentials on a *Clone
    Repository* pop-up window. Provide your GitHub username and PAT (not
    your GitHub password) if prompted.

6.  After a few seconds, your RStudio session will refresh and you
    should be in your newly created RStudio Project!
7.  **ONE TIME ONLY** If you weren’t previously asked to provide your
    GitHub username and PAT, we will attempt to force a prompt so that
    RStudio will not ask for them anymore (wahoo!).

-   Open the `activity02-ggplot2-intro.Rmd` file. This should open on
    the upper-left-hand portion of your RStudio session.
-   In your RMarkdown document, edit the top portion (the YAML) that
    currently says `author: "Name"` so that it contains **your name**
    and save your changes.
-   In the **Git** pane (upper-right-hand pane), select the
    `activity02-ggplot2-intro.Rmd` file and click **Commit**.
-   In the pop-up window, provide a meaningful commit message (e.g.,
    “Add author name”) and click the **Commit** button.
-   Click the
    <img src="README-img/push-icon.png" alt="push" width = "20"/> icon.
    You should be asked for your GitHub credentials - provide your
    GitHub username and PAT. If you were not, RStudio has already stored
    them!

<img src="README-img/noun_pause.png" alt="pause" width = "20"/>
<b>Planned Pause Point</b>: If you have any questions, contact your
instructor or another group.

## ☑️ Task 2: Complete the RMarkdown File

The `activity02-ggplot2-intro.Rmd` file contains the directions for this
activity. For the rest of this class period, you will complete the
RMarkdown document with your neighbor(s). Your instructor will be
circling and be available to help when needed.

Note that each person is working in their own repo. We are not worrying
about collaborating for the time being and instead will be working on
being more comfortable with the workflow for working between RStudio and
GitHub.

However, do not continue in this README document until you and your
neighbor(s) have completed your `.Rmd` files.

![penguin
slide](https://media.giphy.com/media/4KALRmOb8uwbC/giphy.gif "stuck penguin becomes un-stuck")

## ☑️ Tasks 4: Reflection

**YOU DID IT!**

![Vote
Pedro](https://media.giphy.com/media/JJGUejl0pLcRy/giphy.gif?cid=ecf05e474lnk2fbfl0rneodyg95rf1kij3zbsieh46p1cqyb&rid=giphy.gif&ct=g)

Take 5 minutes to write a reflection on what you feel confident in and
what you need to spend some time better understanding. What is one thing
you can do to help clarify your current misunderstandings?

**Next**: Activity 3 will cover the foundational syntax of programming
in R.
