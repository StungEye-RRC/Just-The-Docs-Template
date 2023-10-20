---
title: Home
layout: home
nav_order: 1
---

# The Role of Version Control in Software Development

## Ctrl-Z to Undo
CTRL-Z lets us undo changes in files we have open,
but it has limitations:
- What if you wanted to undo a change to a file you made weeks ago?
- What if you wanted to undo a change made to a file by someone else?
- What if you wanted to experiment with a series of changes and then revert back to a specific version of the file?

## Version Control
**Version control**, also known as **revision control** or **source control**, is the management of changes to documents like computer programs.
CTRL-Z is the simplest form of version control.
**Some documents have more advanced version control built-in:**
- Microsoft Word has a "Track Changes" feature.
- Google Docs automatically tracks file changes over.
- You can see the edit history of all Wikipedia articles. 
[Here's the history of the version control article.](https://en.wikipedia.org/w/index.php?title=Version_control&action=history)

## More Than Just Undo
**Version control allows for more than just undoing things:**
- Work on new projects features while at the same time patching bugs found in older version of the code.
- Collaborate with someone on a projects without overwriting each other's work.
- Work with distributed teams of coders from around the world to develop open-source applications.

## Evolution of Version Control
**A Diary Analogy:**
- **Local Version Control:** Storing your diary under your pillow.
- **Centralized Version Control:** Storing a copy of your diary in a safety deposit box.
- **Distributed Version Control:** Making mulitiple copies to store with trusted friends.

## Why Should I Care About Version Control?
Solo or team, version control is your secret weapon for efficient and stress-free software development.
**It's your development safety net!**

## Different Version Control Systems
**Distributed VCS**
- **Git** - Free. Popular outside of game dev, especially for open source project.
- **Plastic SCM / Unity Version Control** - Paid. Now owned by Unity.
**Centralized VCS**
- **Perforce Helix Core** - Paid. Industry standard for large game dev shops.
- **Subversion** - Free. Classic choice for smaller / indie shops.

## Version Control with Git
- Git is a free and open source distributed version control system.
- Git helps us keep track of the changes to our source code over the lifespan of a project.
- When combined with cloud version control sites like GitHub or GitLab, we can use git to collaborate with others remotely.

## Why Git?
- With Git, you can make a "commit", or a save point, as often as you'd like.
- You can also go back to previous commits. This takes the pressure off of you while you're working.
- Commit often and commit early, and you'll never have that gut sinking feeling of overwriting or losing changes.
- Allows us to work offline if necessarily and synchronize with a distributed team.

## Why Not Git?
**Downsides to working with git in game development:**
- Not especially user friendly for non-developers.
- No built-in support for large repos, although the Git LFS add-on exists.
- No built-in support for locking binary assets. (Locking can be enabled with Git LFS.)

## Some Git Resources
- [Git Guide](https://github.com/git-guides) - Official git Learning Guides from the folks at GitHub.
- [Git CheetSheet](https://training.github.com/downloads/github-git-cheat-sheet/) - The most popular git commands in one page.
- [Pro Git Book](https://git-scm.com/book/en/v2) - Free ebook provides a deep dive into everything git.

## A Brief History of Git
- The Git version control tool was created by Linus Torvalds, the same coder who created the Linux OS.
- Git development started when Bitkeeper, the version control tool being used for Linux development, revoked it's free license for Linux development.
- Development on Git started in April 2005, and by June it was already being used to handle the next Linux kernel release!

## Fancy Version Control Words
- **CLI** - Command Line Interface. The "Terminal" or "Shell" of your operating system. Git is a CLI tool but there are also graphical (GUI) interfaces.
- **Directory** - Used interchangeably with Folder.
- **Repository** - A collection of files and directories you are monitoring for changes using a version control tool. Sometimes shortened to repo.
- **Clone** - Local version of a repo, including all commits and branches.
- **Remote** - Server clone of repo that all team members synchronize to.
- **Graph** - A diagram of nodes connected by lines called edges. (See image below.)
- **DAG** - Directed Acyclic Graph. A graph were the edges are arrows (directed) and no matter which arrow you follow you can never travel in a circle (acyclic).
Example of a DAG:
![Dag](https://ericsink.com/scm/1761_image001.jpg)
- **Hash** - A string of characters that acts like a digital fingerprint for a file or portion of a file. The type of hash used by git is the SHA1 cryptographic hash.
- **Commit** - Snapshot of your entire repository compressed into a SHA.
- **Branch** - A lightweight movable pointer to a set of commits.
- **HEAD** - The HEAD pointer is a reference to the most recent commit in your branch.
- **Working Directory** - The current state of your repo's files on disk.


# Team Members

## Steven
![StevenPhoto](https://avatars.githubusercontent.com/u/144483744?v=4)
This is a short paragraph biography of Steven.

## Olivier


## Russel


## Lorenzo


## Quentin

