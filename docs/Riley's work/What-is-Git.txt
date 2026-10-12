---
title: What Is Git?
layout: default
nav_order: 3
---

# What Is Git?
{: .no_toc }

## Overview

Git is a free, open-source distributed version control system used to track and manage changes to files throughout a project's development.

Git allows developers to save different versions of their projects, restore previous changes, and collaborate with others.

When combined with hosting platforms like GitHub or GitLab, Git also allows developers to share their work with teams remotely.

## Table of Contents
{: .no_toc }

- TOC
{:toc}

## How Does Git Work?

Git tracks changes through repositories, which contain a project's files and their version history.

When developers make changes, they can create a **commit**, which acts as a save point for the project.

Each commit records a snapshot of the project at that point in time, allowing developers to review previous versions and recover earlier work.

Git also supports **branches**, allowing developers to work on new features or bug fixes independently before merging their changes into the main project.

Because Git is distributed, developers can work offline and synchronize their changes with remote repositories when connected.

## Pros of Git

- **Free and Open Source:** Git is available without purchasing a license.
- **Version History:** Developers can create commits and return to previous versions of their projects.
- **Offline Development:** Developers can commit changes and review project history without an internet connection.
- **Branching and Merging:** Developers can experiment with new features without directly affecting the main project.
- **Fast Operations:** Most Git operations are performed locally.
- **Collaboration:** Multiple developers can work on the same project and combine their changes.

## Cons of Git

- **Learning Curve:** Git commands and workflows can be difficult for beginners and non-programmers to understand.
- **Large File Handling:** Git is not optimized for frequently changing large binary assets, although Git LFS can help.
- **Binary File Conflicts:** Files such as textures, models, and audio cannot always be merged automatically.
- **File Locking:** Git does not include built-in file locking, although Git LFS provides locking functionality.
- **Repository Size:** Large projects with extensive file histories can require significant storage space.

## Git in Game Development

Git is useful in game development because programmers and artists often need to collaborate on the same project.

For example, in a Unity project:

- Programmers can track changes to C# scripts and game mechanics.
- Team members can create branches to develop new features independently.
- Developers can restore earlier versions if a new feature introduces bugs.
- Artists can manage textures, models, and audio files, although large assets may benefit from Git LFS.

Git is especially useful for managing code, but game development teams should consider how they will handle large binary files and merge conflicts.

### Practical Example

Imagine a developer wants to experiment with a new enemy AI system without affecting the main project.

They can create and switch to a new branch using:

```bash
git switch -c enemy-ai
```

The developer can then make changes and test the new AI system independently.

Once the feature has been completed and tested, it can be merged back into the main project.

Branching allows developers to experiment with new features while keeping the main project stable.

## Git vs. GitHub

Although Git and GitHub are often used together, they serve different purposes.

- **Git:** A version control system that tracks and manages changes to files.
- **GitHub:** An online platform that hosts Git repositories and provides additional tools for collaboration.

Git can be used entirely on a local computer without GitHub.

GitHub provides features such as pull requests, code reviews, and remote repository hosting that make collaborating with others easier.

## Additional Resources

- [Pro Git - What Is Git?](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F)
- [Pro Git - About Version Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
- [GitHub Docs - About Git](https://docs.github.com/en/get-started/using-git/about-git)
- [GitHub Docs - About Git Large File Storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/about-git-large-file-storage)
- [Unity Documentation - Unity Version Control](https://docs.unity.com/en-us/unity-version-control)
