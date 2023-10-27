---
title: Team Git Workflows
layout: default
nav_order: 10
---
<!-- prettier-ignore-start -->
# Team Git Workflows
{: .no_toc }

Coming with Git, developers have certain workflows or methods or procedures that dictate how developers interact with the Git system for using Git. These workflows are in place to achieve effective team collaboration.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Centralized Workflow
The centralized workflow works by all the developers work directly on one `main` or `master` branch.

That workflow makes it simple and similar to the Subversion-style workflows. the workflow is simple and strait forward, but it isn't as powerful or flexible as other workflows may be. But it is better suited for teams or projects that are smaller so that merging will not become a problem with bigger files and projects when putting it into the main. Although, merging if not done right could be problematic when trying to merge with the main branch of the project.

Centralized workflow would work like this:

1. Initialization: One team member creates the repo with an online remote.
2. Cloning: Each team member then creates a local copy by "cloning" the remote.
3. Working Locally: The developers work on the project, committing to their local repo.
4. Resolving Conflicts: When a developer is then ready to share and push their changes to the remote, they must pull outstanding changes from the remote, and resolve merge conflicts as required.
5. Pushing to Remote: After resolving conflicts, they can now push their changes to the central repo.
6. Synchronizing Team: The other team members can now pull from the central repo to get and implement the latest changes to the project.

## Feature Branch Workflow
For this workflow, this works by having any kind of feature development or any bug fixes will be done all in separate dedicated branches.

Doing this makes any kind of new development in projects isolated from the main branch as well as makes it easy to discard any experimental changes to the project, whatever that may be. This also facilitates code review via pull requests, so somebody needs to take a look at what you are putting into the project before it is able to actually go into the project.

The workflow is similar to the centralized workflow other than:

- Branching: Any new features or fixes are developed locally in a short-lived branch. 
- Resolving Conflicts: Remote commits by other developers can be pulled into the local feature branch, with merge conflicts resolved as required.
- Pushing to Remote: Completed and resolved branches are then pushed.
- Requesting a Remote Merge: A pull request is next initiated on the git hosting service, like GitHub.
- Reviewing: One or more team members then review the pull request before merging it into the main remote branch. Pull requests can be sent back unmerged if the request may need revising or something like that.

## Forking Workflow
This workflow is often used for open source projects, it also makes it so each developer gets not only their own local repo, but also a server-side copy of the project.

By having it like that, developers push to their own sever-side repos. Any changes are shared by pull requests from their own personal public repository. This workflow will need a project maintainer, they will make the final say on what is being merged into the official repo.

How it works is like Feature Branch workflow, but:

- Forking: Each member of the team will create a fork of the project on the git hosting service they are working on.
- Cloning: Then team members clone their remote fork to a local repo on their computers.
- Adding an Upstream: The team members then configure a secondary remote called `upstream` that points to the official repo.
- Resolving Conflicts: Remote commits from `upstream` can be pulled into the local feature branch, with merge conflicts resolved if needed.
- Pushing to Remote: The local feature branches are then pushed to the forked remote.
- Requesting a remote Merge: Finally pull requests are initiated to request any merges from the remote fork to the official upstream repo.
