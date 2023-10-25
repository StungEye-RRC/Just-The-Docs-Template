---
title: Git Life Cycle
layout: default
nav_order: 2
---
<!-- prettier-ignore-start -->
# Git Life Cycle

The Git Life Cycle has four main stages: Untracked, Unmodified, Modified, and Staged. This life cycle shows how changes are recorded in Git.

## Table of Contents 
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

![Git Life Cycle Image](https://courses.csail.mit.edu/6.S194/13/lessons/03-git/img/lifecycle1.png)

## Untracked

In the untracked stage of the life cycle files are not yet being tracked in the repository. You can use `git status` to show which files are not being tracked. To move to the next stage of the Git life cycle you can add files using `git add`. Once added the changes are still not being tracked, in order to move to the next stage of the life cycle and begin tracking changes the file must be committed using `git commit`. Now changes to the file will begin being tracked, and the life cycle has moved to the next stage.

## Unmodified 

Once commited the files are now in the unmodified stage of the cycle. The file can return back to the previous stage by removing the file. In this stage changes will start being tracked, and once a change has occured the file will move to the next stage of the cycle. 

## Modified

Here a file has been changed from its initial commit to the repository. To view changes that have been made to the file you can use `git diff`. Here the changes between your working directory and your staging area are shown. 

## Staged

After the file has been modified it must be readded and commited to the repository. Using `git add` you can stage the files and make a commit using `git commit` this will return the files back to the unmodified stage of the life cycle.

## Additional Resources
[Git add documentiation](https://git-scm.com/docs/git-add)
[Git commit documentation](https://git-scm.com/docs/git-commit)
[Git status documentation](https://git-scm.com/docs/git-status)
[Git diff documentation](https://git-scm.com/docs/git-diff)
