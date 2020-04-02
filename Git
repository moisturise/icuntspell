# Git and GitHub

**Git** is a version control system. It’s software that allows you to keep track of any changes you make to a given project.

**GitHub** is an online platform (https://github.com). It serves two main purposes:

1. GitHub backs up your code. We all know computers are fragile. As I’m typing this lesson, there’s a kombucha sitting awfully close to my Mac. If I were to spill my tea all over my computer, my work wouldn’t skip a beat because I frequently push my projects to GitHub.
1. At its core, GitHub is a social platform. It allows coders to work together on a single project in a highly collaborative fashion.

**GitHub Enterprise** is a private, licenced version of Github, hosted on organisation's own servers.


# Repositories

A **repository** (“repo,” for short) is a project that is under version control.

There are two types of repositories: **local** and **remote**. A local repository is a repo that is stored on your machine, whereas a remote repository is stored online via GitHub.

Some examples:

1. If I start a project on my work computer, but don’t use Git, then my project has no repositories.
1. If I set up my project as a Git repo on my Mac, then my project has a single local repository.
1. If I push my project up to GitHub, my project now has both a local and a remote repository.
1. When I go home, I can download my project from GitHub onto my other computer. My project now has a remote repository and two local repositories.
1. And finally, if I want to test out a competitor to GitHub (i.e., Bitbucket, GitLab, etc.), I can add another remote repository to my project and push my code there. Now my project has two local repositories and two remote repositories.

It’s common to create a new repo for each project you’re working on rather than have several projects lumped into a single repository.

Note: You can use Git without GitHub, in which case you have a **local repo**.


# Installing Git

**PC:**

1. Download and install Git from the official [Git](https://git-scm.com/download/win) website. The download should happen automatically.
1. Once you’ve installed Git, open your **Command Prompt** by:
    1. Hit `<Windows key>`.
    1. Type `<git bash>`.
    1. Press `<enter>`.

**Mac:**

1. Install [Homebrew](https://brew.sh/). Homebrew helps Mac users install various open-source libraries (Python, Git, etc.) with ease. You can read more about Homebrew on its site.
1. Once Homebrew is installed, open your **terminal** by:
    1. Hit `<⌘ (command) + space>`.
    1. Type `<terminal>`.
    1. Press `<enter>`.
1. In your terminal, type `<brew install git>` and press `<enter>`.


# Create a local repository

In your Command Prompt or terminal, first, create a directory (a folder) to house your project. The code below:

1. Change directory `<cd>` to `<Desktop>`.
1. Make a directory `<mkdir>` called `<example1>` that locates on your `<Desktop>`.
1. Change directory `<cd>` to the new folder `<example1>`.

```
cd Desktop
mkdir example1
cd example1
```

To create files `<touch>` for in the directory:

```
touch home.html about.html contact.html
ls
```

When you list `<ls>` items in the directory, you should see something like this (the below example is from a Mac):

```bash
[example1 % ls
 about.html contact.html home.html
 example1 %
```

Now there is a directory on your machine, but it is not a **Git repository** yet. To create an empty Git repository, run:

    git init

When you list all `<ls -a>` items in the directory, you should see something like this (the below example is from a Mac):

```bash
[example1 HEAD % ls -a
 .            .git         contact.html
 ..           about.html   home.html
 example1 HEAD %
```

Git uses `<.git>` as a log to keep track of changes. Now you have a local repository for your project `<example1>`.


# Adding Files to the Repository

Type the following in your terminal:

```bash
git status
```

Use `<git status>` regularly to keep track of what Git has saved. Now it shows you that the three files are currently not being tracked by Git, even though they are in the project directory. You need to tell Git to keep track of any changes made to these files by running:

```bash
git add about.html
```

Run `<git status>` and you can see that Git starts tracking changes you make to `<about.html>`, but not `<contact.html>` and `<home.html>`.

To add all of the files in the current directory `<.>` to Git, run:

```bash
git add .
```

`<.>` is the current directory. In this case, the current directory is `<example1>`. Run `<git status>` and you should see there is no `<Untracked files>`.

Now all three files are tracked by Git, we should save in Git.


# Saving in Git

run `<git log>` in your terminal, you should see `<fatal: your current branch 'master' does not have any commits yet>`.

Each change made in Git is a `<commit>`. The message means that nothing has been saved yet.

To create your first commit and to check the status, run:

```bash
git commit -m"Created about.html, contact.html and home.html"
git status
```

Start your commit message with `<-m>` flag. Your commit message should record what change you have made. Wrap the commit message in quotation marks, “Created about.html, contact.html and home.html”. You can find some helpful tips on commit message best practice online. For example, the [commit message guidelines](https://gist.github.com/robertpainsi/b632364184e70900af4ab688decf6f53) here is quite good. Committing your changes to Git is a fundamental concept. Git is all about version control.

Run `<git log>` to check your commit history, you should see your first commit in the timeline now.
