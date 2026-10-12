---
title: Repository Initialization
parent: Git Fundamentals
nav_order: 2
layout: default
---

# Repository Initialization

This page will go over how to create a repository through Windows Terminal/GitBash

## Table of Contents
{: .no_toc}
1. TOC
{:toc}


## Initialization

To bring a new project under control we must first initialize the repository (the repo)
from within the project's root folder:

To initialize a new git repo from the command prompt:
```
git init .
```

Git defaults to using the word "master" (as in "master copy" or "master recording") for
the main branch, but we can change this:
```
git branch -m main
```

 
