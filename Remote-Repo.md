---
title: Remote Repositories
layout: default
nav_order: 8
---

# Why Create a Repository?
{: .no_toc }

A repository is a place where you store and manage your project's files, including its code and documentation. There are many reasons to create a repository. For example, if you are making a website and need to collaborate with other programmers, creating a remote repository makes it much easier to work together. A remote repository is a version of your project stored on a server or cloud platform, such as GitHub. It allows multiple programmers to access the same project without having to manually send files back and forth.

## Table of Contents
{: .no_toc }
1. TOC
{:toc}


## Version Control

One of the main reasons to create a repository is to use version control. Version control tracks changes made to your project over time. This allows you to see previous versions of your code and return to an earlier version if something breaks.

For example, if you accidentally delete an important function, you can use Git to find the previous version and recover your work.

## Collaboration

Repositories make it easier for multiple programmers to work on the same project. Using a remote repository, team members can upload their changes, download updates from others, and work on separate features.

Git also allows programmers to create branches. A branch lets someone work on a feature without directly changing the main version of the project. Once the feature is complete, the changes can be reviewed and merged into the main branch.

## Backing Up Your Project

A remote repository can act as a backup of your project. If your computer breaks or you lose your local files, you can download the project again from the remote repository.

However, this only protects files that have been committed and pushed to the remote repository. Changes that exist only on your computer will not be backed up remotely.

## Tracking Changes

Repositories help you keep track of changes made to your project. Git records commits, which are saved snapshots of your work. Each commit can include a message explaining what was changed.

For example, a commit message might be `Fixed player movement` or `Added login screen`. These messages help you and your teammates understand how the project has developed over time.

## Useful Git Commands

The following commands are useful when creating and working with repositories.

- `git init` — Creates a new local Git repository.
- `git clone <repository-url>` — Downloads an existing remote repository to your computer.
- `git add .` — Stages changes so they can be included in a commit.
- `git commit -m "Your message"` — Saves staged changes as a commit.
- `git push` — Uploads committed changes to a remote repository.
- `git pull` — Downloads and integrates changes from a remote repository.

