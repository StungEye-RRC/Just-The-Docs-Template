---
title: The Role of Version Control in Software Development
layout: default
nav_order: 2
---

# The Role of Version Control in Software Development
{: .no_toc }

## Overview

Version control, also known as revision control or source control, is the management of changes to documents such as computer programs.

In software development, it helps developers manage different versions of a project, collaborate with others, recover older versions, and safely test new features.

Unlike simply using `Ctrl + Z`, version control allows developers to undo changes made weeks ago, restore older versions of files, and manage changes made by other team members.

## Table of Contents
{: .no_toc }

- TOC
{:toc}

## Pros of Version Control

Version control provides developers with much more than just the ability to undo changes.

- Tracks changes made to a project over time.
- Makes it easy to restore older versions of files.
- Allows developers to work on new features while fixing bugs in older versions.
- Helps multiple developers collaborate without overwriting each other's work.
- Allows distributed teams to work together on projects from anywhere in the world.
- Makes testing new features safer.
- Helps identify when bugs were introduced.

Version control is useful for both individual developers and teams, providing a safety net throughout the development process.

## Types of Version Control

### Local Version Control

Stores different versions of files on one computer. It is simple, but not ideal for team projects.

### Centralized Version Control

Stores the main project on a central server. Developers connect to the server to access and update files.

Examples include:

- Perforce Helix Core
- Subversion (SVN)
- CVS

### Distributed Version Control

Each developer has a full copy of the project and its history. Developers can work independently and then synchronize their changes.

Examples include:

- Git
- Mercurial
- Unity Version Control (formerly Plastic SCM)

## Version Control in Game Development

Version control is especially useful in game development, where programmers and artists often work on the same project.

For example, in a Unity project:

- Programmers can track changes to scripts and game mechanics.
- Artists can manage changes to textures, models, and other assets.
- Team members can work on different features without directly overwriting each other's work.
- Developers can restore earlier versions if a new feature introduces problems.

Different version control systems are commonly used in game development:

- **Git:** A free, open-source distributed version control system, commonly used in software development and smaller game projects.
- **Unity Version Control:** A version control solution designed for game development teams, including programmers and artists.
- **Perforce Helix Core:** A centralized version control system widely used by larger game development studios.
- **Subversion (SVN):** A centralized version control system that can be used by smaller development teams.

### Practical Example

Git allows developers to view the history of changes made to a project.

Inside an existing Git repository with commits, run:

```bash
git log --oneline
```

This displays a shortened history of commits, including their identifiers and messages.

This can help developers identify when a particular feature was added or a bug was introduced.

In game development, being able to see a log of commits helps dramatically with bug fixing, as teams can work backwards to find possible sources of an issue.

## Brief History

Early developers often saved multiple copies of files manually to keep older versions.

I remember back in high school when my team didn't know how to use version control. We used flash drives to share, merge, and keep track of different versions of our projects.

As software projects became larger, version control systems such as SCCS and CVS were created to track changes more reliably.

Centralized systems such as SVN later became common for team development.

Git was created by Linus Torvalds, the creator of Linux, in April 2005 after the version control system BitKeeper stopped providing free licenses for Linux development.

By June 2005, Git was already being used to manage development of the Linux kernel.

Today, Git is one of the most widely used version control systems in software development and is also used in game development.

## Additional Resources

- [Pro Git - About Version Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
- [GitHub Docs - About Git](https://docs.github.com/en/get-started/using-git/about-git)
- [Pro Git - A Short History of Git](https://git-scm.com/book/en/v2/Getting-Started-A-Short-History-of-Git)
- [Git Documentation - git log](https://git-scm.com/docs/git-log)
