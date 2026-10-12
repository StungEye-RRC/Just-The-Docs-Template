---
title: Staging and Commiting
parent: Git Fundamentals
nav_order: 3
layout: default
---

# Staging and Commiting Files

In order to upload files and changes to files to a remote repository, they must first be staged and then commited.

## Table of Contents
{: .no_toc}
1. TOC
{:toc}



## Staging

To see what files are currently unstaged, you can run the command:

```
git status
```

To stage a specific file:

```
git add filename
```

To stage all currently unstaged files:

```
git add .
```


## Commiting

After staging your files, you can commit them with:

```
git commit -m "commit message"
```

When commiting, make sure your commit message specifies what you changed exactly. This is useful for
- Traceability: Commit messages clarify code history and aid in debugging.
- Collaboration: They help others understand the intentions behind changes.
- Documentation: They act as a form of source code documentation.
- Change Management: - "Change Logs" based on commits are often shipped with each release.

