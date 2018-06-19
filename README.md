# Forking and Cloning Github Repositories

## Problem Statement

It will be important to get used to forking and cloning repos. Both are `git` functions
that allow a user to make copies of the repo, but can serve different functions, depending
on what needs to be done. If you're working on a repository that you don't have "write"
access to, such as Flatiron School's `github.com/learn-co-students/` repo, you may find
yourself cloning a readme or lab to your local environment, but being unable to submit
your changes with a `git push`. How are you able to keep track of your changes that are
being added to a repo you're working on? This is where you would use `git fork` and make
a clone of that instead!

## Objectives

1. Use `git fork` to copy a repo
2. Use `git clone` to save a repo to your local machine

## Use `git fork` to Copy a Repo

Forking a GitHub repository is just a way to create your own copy of it. For those 
who have been using the in-browser Learn interface-- this is a common action that is
taken. Each time you fork a lab, GitHub creates a copy that you can use as a 
sandbox to play around in, while maintaining a canonical repo where the original lab/content
remains intact. In other words, forking creates another copy that allows you to work in your 
own world without messing with the core content.

![Fork Button](http://readme-pics.s3.amazonaws.com/fork_button.jpg)

Outside of Learn, forking is a very commonn workflow for working with teams or
working with or contributing to open sourced content in the Github community.
You can fork any repo by clicking the "Fork" button at the top right of any
GitHub repository. For labs and code alongs, the Learn interface simplifies this
process by allowing you to click the "OPEN IDE" button at the top of any lab (if 
you use the Learn IDE) or to type `learn open` in your terminal (if you use
a local development environment). In both cases, the GitHub repository will be
automatically forked and cloned.

Instead of automating the process as we have been doing, for this lesson, we're
going to manually fork and clone, so to get started, click the GitHub icon at
the top of this page:

![github button](https://s3.amazonaws.com/flatiron-client-assets/assets/github-learn-button.png)

This will bring you to the "learn-co-students" version of this lesson.  Click
the 'Fork' button in the upper right corner of the page.  You will be prompted
to choose where the repository should be forked to, so go ahead and choose your
account.  GitHub will take a few moments to create the fork, then navigate to
your copy of the repository.  If all has gone well, you will see your username
at the top of the page, followed by a `/` and the name of the repository, along
with a link just below to the original repository.

For the lessons on learn.co, it's worthwhile to note that you can go back and
forth between the original repo and your fork by changing your GitHub username
within the GitHub URL to "learn-co-students". For example:

```
https://github.com/your-username-here/forks-and-clones-readme-v-000
```
Change to your-username-here to "learn-co-students":
```
https://github.com/learn-co-students/forks-and-clones-readme-v-000
```

[More on forking in the GitHub docs.](https://help.github.com/enterprise/2.2/user/articles/fork-a-repo/)

## Use `git clone` to Save a Repo to Your Local Machine

Now we want to get our forked copy of the repository on our local machine. This
is where cloning is useful. To do this:

1. Navigate back to the forked repository page you just created on GitHub.
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

This will create a local copy of our forked GitHub repository. And that is it!

## Conclusion

Github gives developers many ways to collaborate. Using `git fork` and `git clone` 
in conjunction allow you to work independently and collaboratively on repos you 
may not have direct access to edit. Note that this is something you can do on
_any_ public GitHub repository, not just Learn lessons.  So if you've found
a GitHub repository that you'd love to build off of or modify for your own use,
you can use this process to make your own copy.  Often, the original authors
will include license information regarding how you can use their repository,
so make sure to check before you publish, sell or distribute any material
you've forked, cloned and modified. 

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/forks-and-clones-readme' title='Forks and Clones'>Forks and Clones</a> on Learn.co and start learning to code for free.</p>

<p class='util--hide'>View <a href='https://learn.co/lessons/forks-and-clones-readme'>Git Forks and Clones</a> on Learn.co and start learning to code for free.</p>
