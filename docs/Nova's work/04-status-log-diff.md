---
title: Status, Log, and Diff
parent: Git Fundamentals
nav_order: 4
layout: default
---

# Status, Log, and Diff

This section will go over Status, Log, and Diff and what they do.

## Table of Contents
{: .no_toc}
1. TOC
{:toc}


## Status

Status allows you to see the current status of all tracked files. The command for this is:
```
git status
```


## Log

Log allows you to see a list of every commit. The command for this is:
```
git log
```

Each entry in the log shows:
- The commit hash.
- Who made the commit.
- When it was made.
- The commit message.


## Diff

Diff is used compare the differences between the current files and the last commit:
```
git diff
```

We can also diff specific files:
```
git diff secret_plans.tx
```

Or specific folders (and their sub-folders):
```
git diff ./textfiles/plans
```