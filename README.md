# Forking and Cloning GitHub Repositories

## Problem Statement

If you are familiar with how to create local repositories, you have the ability
to create a logged history of your project.

What's great about `git` and open source is that lots of people are _doing the
exact same thing_ all around the world all the time.

In this lesson we'll learn how to acquire others' repositories. In a subsequent
lesson we'll cover how to push our locally-created repositories onto the
internet. Let's learn to acquire others' code!

## Objectives

1. Define _remote_
2. Use `git clone` to copy a repository to your local machine
3. Use `git remote` to list remotes
4. Use `git fork` via GitHub to duplicate other organization's repositories into your own

## Define _remote_

To work with or collaborate on any `git` project, you need to be able to manage
your _remote_ repositories. Remote repositories are versions of a repository
that are hosted online, typically, on GitHub.

## Use `git clone` to Copy a Repository to Your Local Machine

We use `git clone` to copy someone else's remote copy of their local repository
to our machine.

1. Navigate to the https://github.com/facebook/react repository
2. Click the "Clone or Download" green button on the right.
2. Make sure you select `Use SSH` as your URL type.

	![SSH URL](https://files.readme.io/UgsI2ndmR2aH5ky5G1OA_GitHub%20-%20SSH%20-%201.png)

3. Click the "Copy to clipboard" button (highlighted below). This will copy the
URL for us to use when we clone.

	![Clone Repo Button](http://readme-pics.s3.amazonaws.com/clone-repo-clone-url-button.png)

4. In the terminal (accessed through the 'Sandbox' or Learn IDE), we need to
run the `git clone` command. It takes the URL we just copied as an argument,
like so:

	```bash
	git clone your-copied-github-url
	```

This will create a local copy of our forked GitHub repository.

## Use `git remote` to List Remotes

If you use the `ls` command, you'll see `git` created a directory called
`react`. Use `cd` to enter that directory.

```bash
cd react
```

Type `git remote` to see each remote available.

If you've cloned your repository, you should at least see `origin`. The remote
called `origin` is the default name `git` gives to the remote you cloned from:

```bash
$ git remote
origin
```

## Use `git fork` via GitHub to Clone Other Organization's Repositories Into Your Own.

Forking a GitHub repository is just a way to create a personal, online duplicate
of it. When you fork a lab, GitHub creates a duplicate from the source
organization's online version of the repository to **your** local duplicate of the
repo.

It's like saying "Hey, can I have the Louvre's version of _The Mona Lisa_?" The
Louve would say no. If you were to create an exact online duplicate by
_forking_ it from `louvre/mona_lisa` to `your-name/mona_lisa` the Louvre would
be cut out of the, pardon the pun, picture. You could then copy *your*
organization's version to *your* local machine with `git clone`.

![Fork Button](http://readme-pics.s3.amazonaws.com/fork_button.jpg)

Forking is a very common workflow for working with teams or working with or
contributing to open sourced content in the GitHub community.  You can fork any
repository by clicking the "Fork" button at the top right of any GitHub
repository.

Let's try a fork and clone workflow.

Click the GitHub icon at the top of this page:

![github button](https://s3.amazonaws.com/flatiron-client-assets/assets/github-learn-button.png)

This will bring you to the "learn-co-students" version of this lesson.  Click
the 'Fork' button in the upper right corner of the page.  You will be prompted
to choose where the repository should be forked to, so go ahead and choose your
account. GitHub will take a few moments to create the fork, then navigate to
your copy of the repository.  If all has gone well, you will see your username
at the top of the page, followed by a `/` and the name of the repository, along
with a link just below to the original repository.

[More on forking in the GitHub docs.](https://help.github.com/enterprise/2.2/user/articles/fork-a-repo/)

The important take away is to **not** misuse "fork" and "clone" when speaking
with other `git` users. To get a local copy: **clone**; to make an online copy
of a repository to your personal organization so that you have the ability to
update its `master` branch, **fork**.

## Conclusion

GitHub gives developers many ways to collaborate. Using `git fork` and `git
clone` in conjunction allow you to make local copies of others' code. As you
saw with cloning React, this is something you can do on _any_ public GitHub
repository.  So if you've found a GitHub repository that you'd love to build
off of or modify for your own use, you can use this process to make your own
copy.  Often, the original authors will include license information regarding
how you can use their repository, so make sure to check before you publish,
sell or distribute any material you've forked, cloned and modified.

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/forks-and-clones-readme' title='Forks and Clones'>Forks and Clones</a> on Learn.co and start learning to code for free.</p>

<p class='util--hide'>View <a href='https://learn.co/lessons/forks-and-clones-readme'>Git Forks and Clones</a> on Learn.co and start learning to code for free.</p>
