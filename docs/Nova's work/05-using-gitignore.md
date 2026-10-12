---
title: Using a Git Ignore File
parent: Git Fundamentals
nav_order: 5
layout: default
---

# Using a Git Ignore File

Sometimes there are files you don't want to include in your repo:
- Files that include secrets like passwords or API keys.
- Temporary files and folders.
- Build files and folders.
- Hidden OS files like .DS_Store (Mac) or Thumbs.db (Windows) files.

You can make Git ignore these files using a .gitignore file.

## Table of Contents
{: .no_toc}
1. TOC
{:toc}


## Git Ignore File

Exclude files and folders by creating a .gitignore file in the project root.

Here some examples of how to ignore files:
```
# Ignore specific files. (Note that comments start with: #)
Thumbs.db
# Wildcards: Ignore all .exe files.
*.exe
# Exception to wildcards: Do track the special.exe file.
!special.a
# Ignore all files in any folder called build.
build/
# Ignore all .pdf files in the doc/ folder and any of its sub-folders.
```
