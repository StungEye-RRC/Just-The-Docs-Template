---
title: Git Reset
layout: default
parent: Undoing in Git
nav_order: 2
---

# When to Undo with Reset?

Use `git reset` to undo one or more commits in our local repository.

***WARNING:*** *Dangerous. The rewrites history by changing the HEAD pointer.*

A `git reset` comes in two main flavors:

- Hard Reset (Dangerous)

- Soft Reset (Weird)

(There's also mixed reset, but [I'll leave that up to you to research.](https://practicalseries.com/1002-vcs/02-05-concept.html#js--020505))

## Hard Reset

**Hard Reset:** Changes your working directory to match a specific commit.

`git reset --hard [commit id]`

***WARNING:*** *Uncommitted changes lost. All files are reset to the specified commit!*

## Soft Reset

**Soft reset:** Keeps your changes in the working directory, but still resets the HEAD.

`git reset --soft [commit id]`

***WEIRD:*** *HEAD and your working directory may differ if you have uncommitted changes.*

## Before Reset: HEAD at D

![Before Reset, Head at D](https://i.imgur.com/YRVmxmG.png)


Let's say we want to undo the changes made in C and D:

`git reset --hard B`

### After Reset: HEAD at B

![After Reset, Head at B](https://i.imgur.com/CTVwJ1w.png)

### No Commits Were Lost

`git reset --hard D`

![Before Reset, Head at D](https://i.imgur.com/YRVmxmG.png)
