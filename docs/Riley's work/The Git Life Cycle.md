---
title: The Git Life Cycle
layout: default
nav_order: 3
---

# The Git Life Cycle
{: .no_toc }

## Overview

The Git life cycle describes how files move through different states as changes are made and committed to a repository.

Git uses three main areas to manage changes: the Working Directory, Staging Area, and Git Repository.

## Table of Contents
{: .no_toc }

- TOC
{:toc}

## The Three Main Areas

### Working Directory

The working directory is where developers create, edit, and delete project files.

Changes made here are not automatically saved to Git's commit history.

### Staging Area

The staging area, also called the index, is where developers prepare changes for their next commit.

Using `git add`, developers can choose which changes they want to include in a commit.

### Git Repository

The Git repository stores the committed history of a project.

Each commit records a snapshot of the staged changes along with information such as the author, date, and commit message.

## The Four File States

Throughout the Git life cycle, files can move between four common states:

- **Untracked:** A new file that Git is not yet tracking.
- **Unmodified:** A tracked file that has not changed since its last committed version.
- **Modified:** A tracked file that has been changed but has not had its latest changes staged.
- **Staged:** A file whose changes have been prepared for the next commit.

After committing, staged changes become part of the repository's history. If the working file has no additional changes, it returns to the unmodified state.

## Git Life Cycle Commands

The following commands are commonly used when moving through the Git life cycle:

| Command | Purpose |
|:---|:---|
| `git status` | Displays the current state of files in the repository. |
| `git add <filename>` | Stages a file for the next commit. |
| `git add .` | Stages changes in the current directory and its subdirectories. |
| `git commit -m "message"` | Saves staged changes as a new commit. |
| `git log` | Displays the repository's commit history. |

## Git Life Cycle in Game Development

The Git life cycle is especially useful when developing games with multiple programmers and artists.

For example, when working on a Unity project:

1. A programmer creates or modifies a C# script in the working directory.
2. The programmer uses `git status` to check which files have changed.
3. The script and any required `.meta` files are staged using `git add`.
4. The programmer creates a commit with a descriptive message.
5. Git records the changes in the repository's history.

This process allows developers to keep track of changes made to scripts, scenes, and other game assets throughout development.

### Practical Example

Imagine a developer has finished implementing a player's jump mechanic in Unity.

First, check the current state of the repository:

```bash
git status
```

Stage the modified script:

```bash
git add Assets/Scripts/PlayerMovement.cs
```

Commit the changes:

```bash
git commit -m "Add player jump mechanic"
```

The changes are now recorded in the local repository's history.

You can view the commit using:

```bash
git log --oneline
```

**Note:** If a file is modified after staging, it must be staged again to include those latest changes in the commit.

## Additional Resources

- [Pro Git - Recording Changes to the Repository](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository)
- [Pro Git - What is Git?](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F)
- [Git Documentation - git status](https://git-scm.com/docs/git-status)
- [Git Documentation - git add](https://git-scm.com/docs/git-add)
