---
title: Undoing in git 
layout: default
nav_order: 15
---

# Undoing in git
{: .no_toc }

## Overview

With git, ALMOST anything can be undone.

There are 3 normal ways to undo in git.
- Checkout (Slightly Dangerous)
- Reset (Destructiive)
- Revert (Safe)

## Table of Contents
{: .no_toc }

- TOC
{:toc}

## When to Undo with Checkout?
The simplest private undo. Discard uncommitted local changes

```bash
git checkout <path-or-filename>
```

Works if:
- The changes you wish to undo haven't yet been committed. (Dirty files.)
- You wish to revert to the most recently committed version of a file or files.

## Undoing with Checkout
Let's say you made a bunch of changes to your `readme.md` that you now regret.

If you haven't committed these changes, you can undo them like this:
```bash
git checkout readme.md
```
If you want to revert all folders and files to the most recent commit:
```bash
git checkout .
```
WARNING: Slightly dangerous. The discarded changes cannot be recovered!

## When to Undo with Reset?
Use `git reset` to undo one or more commits in our local repository.

WARNING
: Dangerous. The rewrites history by changing the HEAD pointer.

A `git reset` comes in two main flavors:

Hard Reset (Dangerous)
Soft Reset (Weird)

Aswell as a mixed reset.

## Hard Reset
Hard reset: Changes your working directory to match a specific commit.

```bash
git reset --hard [commit id]
```
WARNING: Uncommitted changes lost. All files are reset to the specified commit!

## Soft Reset 
Soft reset: Keeps your changes in the working directory, but still resets the HEAD.

```bash
git reset --soft [commit id]
```
WEIRD: HEAD and your working directory may differ if you had uncommited changes. 

## Mixed Reset
Mixed reset: Moves HEAD back and unstages the changes, but keeps them in the working directory.

```bash
git reset [commit id]
```

NOTE: This is the default mode, so `--mixed` is optional. The undone commits' changes show up as dirty files, ready to be edited, re-staged with `git add`, and recommitted.

WARNING: Don't reset commits you've already pushed. It rewrites history. Use `git revert` instead.

### Before Reset: HEAD at D
`main --> A --> B --> c --/ D`

Let's say we want to undo the changes made in C and D:
```bash
git reset --hard B
```
### After Reset: Head at B 
`main --> A --/ B`
### No Commits Were Lost
```bash
git reset --hard D
```
###  Back to Where we Started
`main --> A --> B --> c --/ D`

## When to Use Revert?
Use `git revert` to run a specific commit in reverse.

Typically used to undo a commit that has been shared with others.
The public undo - it says, 'I made a mistake, but I want to keep a record of it.'

## Reverting Commits
```bash
git revert <commitid>
```
Creates a new commit that undoes changes from the specified commit.

### The Safest Undo Choice!

Reverting maintains history, making it a safe choice for:
- Undoing local commits.
- Undoing commits pushed to a remote repo.

### Before Revert: HEAD at D
`main --> A --> B --> C --/ D`

If we wish to revert the changes made in D:
```bash
git revert D
```
### After Revert: HEAD at E
`main --> A --> B --> C --> D --/ E`
E (Undoes Changes Made in D)


## Reverting Multiple Commits

The `git revert` command reverts a single commit by default.

We can run it mutiple times to revert multiple commits:
```bash
git revert D
git revert C
```
Or we can revert a sequence of commits:
(Each commit is reverted separately!)
```bash
git revert C^..D
```
If you only want a single revert commit:
(The -n stands for "no commit".)
```bash
git revert -n C^..D
git commit -m "Revert commits C through D inclusively."
```

## Undo: A Decision Tree

`So You Want To Undo --> Changes Committed?`

`Changes Committed? --NO--> Use git checkout, carefully`

`Changes Committed? --YES--> Changes Pushed?`

`Changes Pushed? --YES--> Use git revert`

`Changes Pushed? --NO--> Live Dangerously?`

`Live Dangerously? --NO--> Use git revert`

`Live Dangerously? --YES--> Use git reset`

NOTE: The `git clean` command can also be handy when you want to discard all files that are not under version control.