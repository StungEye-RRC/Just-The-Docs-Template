---
title: Home
layout: home
nav_order: 1
---

## What is _Version Control_?
Version control software keeps track of every modification to the code in a special kind of database.
If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.


## What is _Git_?

By far, the most widely used modern version control system in the world today is Git. Git is a mature, actively maintained open source project originally developed in 2005 by Linus Torvalds, the famous creator of the Linux operating system kernel.

Pros of using Git:
 - It's really quick
 - Local commits rock
 - Quick to start a new repository (no configuration etc)
 - github is easy to use

Cons of using Git:
 - Lack of IDE and Explorer integration
 - Cannot checkout a part of the repository
 - Does not track empty folders
 - Bad Windows support


## What are _Tags_ in Git?

Git tags are a way of labelling specific commits. This can be used for organization and documentation, such as marking specific versions of your repository with descriptive labels (example: `v0.12.4`). There are two kinds of tag, a lightweight tag, which is just a label, and an anotated tag, which contains metadata such as who added the tag, when it was added, and an associated message.
To add a tag to a commit, you can use the terminal command `git tag [tag name] [commit hash]`. If the commit hash is left out, the tag will be applied to the head of the repository. To create an anotated tag instead of a lightweight one, the `-a` parameter can be added between `tag` and `[tag name]`. Note that if the `-m` parameter as well as a message is not provided, a text editor will be opened so you can provide the message at that time.
Tags can also be used in place of the hash for the commit they are associated with in various git commands that can take in commit hashes. By default they are not pushed to remotes with the `git push` command, but can either be passed explicitly (example: `git push origin v0.12.4`) or pushed by adding the `--tags` argument to a push command.


## What is _Stashing_ in Git?

Stashing is a way of hiding away changes made to a repository either to be added to a later commit, or brought to another branch. The stash functions like stacking papers, where the most recently added items are the ones that will be removed first.
To put a set of changes on the stash, you can use the terminal command `git stash push`.
To retrieve a set of changes, you can use the terminal command `git stash pop` or alternatively `git stash show` to preview the changes, followed by `git stash apply` to apply the previewed changes onto the current branch.

The `push` command can be used alongside several optional parameters such as:
 - `-a`/`--all`: any ignored or untracked files in the repository are added to the stash and removed from the repository
 - `-u`/`--include-untracked`: includes untracked files, which are then removed from the reopsitory
 - `-s`/`--staged`: only pushes staged filed to the stash. Basically works like a commit to the stash instead of the current branch


# Team Biography

**Aiden**
- Aiden is a programmer and web developer, who enjoys gardening, playing games, and going out with friends.

**Cole**
 - write yours here

**Spike**
 - write yours here

**Santiago**
 - Is a programmer with experience in Java, Python, and C#. He enjoys biking, running, and playing a variety of games

**Alex**
 - write yours here
