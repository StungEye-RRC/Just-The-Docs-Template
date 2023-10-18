---
title: Branches
layout: default
nav_order: 5
---

<!-- prettier-ignore-start -->
# Branches
{: .no_toc }

In Git, branches are like alternate timelines in a sci-fi movie.They allow you to work on different features or fixes without affecting the main project timeline until you choose to merge the timelines back together.

![Diagram of branches](<https://github.com/CraigRRC/GitWikiGroup1/tree/main/photos/Screenshot%202023-10-18%20143317.png>)

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Creating Branches

**Creating a new branch:**
```
git branch <branch-name>
```
**Switching to a branch:**
```
git checkout <branch-name>
```
**Create and switch in a single command:**
```
git checkout -b <branch-name>
```

## Merging Branches
Branching allows for isolated development, and merging brings those developments
back into the main timeline.

Let's say we've been working and committing to an experimental branch and we
want to merge those commits back into main:
```
git checkout main
git merge experimental
```

