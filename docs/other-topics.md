---
title: Other Topics
layout: default
nav_order: 10
---
<!-- prettier-ignore-start -->
# Other Topics
{: .no_toc }

Now that you've learned the basics of Git, here are some advanced and interesting topics about git for you to git into.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Switch
This is a command that can be used interchangably with `git checkout` for switching branches.
`git switch "develop"` will switch you to the branch named "develop"
`git switch -c "Feature"` will create a branch named Feature, and then switch to the newly created feature branch.

## [Rebasing](https://git-scm.com/book/en/v2/Git-Branching-Rebasing)
The git rebase command lets us modify the commit history by moving or combining a sequence of commits to a new base commit.

## [Cherry-Picking](https://git-scm.com/book/en/v2/Distributed-Git-Maintaining-a-Project#_rebase_cherry_pick)
This is a powerful command that enables arbitrary Git commits to be picked by reference and appended to the current branch.

## [Bisecting](https://git-scm.com/docs/git-bisect)
Git bisect is a binary search algorithm for finding the commit that introduced a bug.

## [Reflog](https://git-scm.com/book/en/v2/Git-Internals-Maintenance-and-Data-Recovery#_data_recovery)
Git includes a reference log or "reflog" - a log of where your HEAD and branch references have pointed.

## [Submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules)
Submodules allow you to keep a Git repository as a subdirectory of another Git repository.

## [Hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks)
Hooks are scripts that Git executes before or after events such as: commit, push, and receive.

## [Git Large File Storage (LFS)](https://git-lfs.com/)
Git extension to allow the versioniong of large files. 

## Additional Resources
[Switch](https://git-scm.com/docs/git-switch)