---
title: Push and Pull
layout: default
nav_order: 10
---

# Pushing and Pulling
{: .no_toc}

Pushing and pulling are two important Git operations used to keep your local repository and your remote GitHub repository up to date. Pushing uploads your committed changes to GitHub, while pulling downloads and integrates changes from GitHub into your local project. These commands are especially useful when collaborating with other programmers.

## Table of Contents
{: .no_toc}

1. TOC
{:toc}

## Pushing Changes

Pushing sends your committed changes from your local repository to your remote repository on GitHub. This allows you to save your work online and share it with other programmers.

To push your changes for the first time, use this command

```bash
git push -u origin main
```

Here is what each part means.

- `git push` uploads your committed changes to the remote repository.
- `-u` sets the upstream connection, linking your local branch to its remote branch.
- `origin` is the name of your remote repository.
- `main` is the name of the branch you are pushing.

Once the upstream connection has been set, you can usually upload future changes by simply using:

```bash
git push
```

Before pushing, you need to stage and commit your changes. Git does not automatically upload uncommitted files.

## Pulling Changes

Pulling downloads changes from your remote repository and brings them into your local branch. This is useful when another coder has uploaded changes or when you have updated your project from another computer.

To pull changes from GitHub, use this thing.

```bash
git pull
```

If your local branch is already connected to its remote branch, Git will know where to retrieve the changes from.

If you need to specify the remote and branch manually, use this.

```bash
git pull origin main
```

This tells Git to pull changes from the `main` branch of the remote named `origin`.

Git will attempt to integrate the downloaded changes into your current branch. If the changes conflict with your local work, you may need to resolve merge conflicts before continuing.

## Common Issues

### Push Rejected

Sometimes Git may reject a push because the remote repository contains changes that your local repository does not have.

You may need to pull the latest changes, resolve any conflicts, and then push again.

### Merge Conflicts

A merge conflict happens when Git cannot automatically combine changes made to the same part of a file.

You must manually resolve the conflicting changes, save the file, and commit the resolution before pushing.

## Useful Git Commands

Here is a quick reference for the commands covered on this page.

`git push -u origin main` Push changes and set the upstream connection.
`git push`  Push changes to the connected remote branch. 
`git pull`  Download and integrate changes from the connected remote branch. 
`git pull origin main`  Pull changes from the remote `origin` and its `main` branch. 
`git branch`  Display your local branches. 
