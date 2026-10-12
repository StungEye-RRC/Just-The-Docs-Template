---
title: Resolving Merge Conflicts
layout: default
nav_order: 7
---

# Resolving Merge Conflicts
{: .no_toc }

## Overview

A merge conflict occurs when Git cannot automatically combine changes from two branches.

This commonly happens when multiple developers edit the same lines of a file differently, or when one developer modifies a file that another has deleted.

When a conflict occurs, Git pauses the merge and requires the developer to manually resolve the conflicting changes before continuing.

## Table of Contents
{: .no_toc }

- TOC
{:toc}

## Why Do Merge Conflicts Happen?

Git can normally combine changes made to different parts of a project automatically.

However, when two branches contain incompatible changes, Git may not be able to determine which version should be kept.

Common causes include:

- Two developers modifying the same lines of code differently.
- One developer deleting a file that another has modified.
- Multiple developers making conflicting changes to shared project files.
- Two artists modifying the same binary asset, which Git cannot automatically combine.
- Having an assignment that requires merge conflicts to occur...

## Understanding Merge Conflict Markers

When a merge conflict occurs in a text file, Git inserts special markers to identify the conflicting sections.

The three main markers are:

- `<<<<<<< HEAD` - Marks the beginning of changes from the current branch.
- `=======` - Separates the changes from the two branches.
- `>>>>>>> branch-name` - Marks the end of changes from the incoming branch.

### Practical Example

Imagine two developers have modified the same variable in a Unity C# script.

When merging their branches, Git might display:

```csharp
<<<<<<< HEAD
float moveSpeed = 5f;
=======
float moveSpeed = 8f;
>>>>>>> feature/player-movement
```

The current branch uses a movement speed of `5f`, while the incoming branch uses `8f`.

The developer must decide which value to keep or combine the intended changes.

For example, if the correct value is `8f`, the resolved code would be:

```csharp
float moveSpeed = 8f;
```

All conflict markers must be removed before completing the merge.

## How to Resolve Merge Conflicts

### Step 1: Identify Conflicting Files

When a merge fails, Git alerts the developer that a conflict has occurred.

Use the following command to identify files containing unresolved conflicts:

```bash
git status
```

Conflicting files will appear under the unmerged paths section.

### Step 2: Resolve the Conflicting Changes

Open each conflicting file in a text editor and locate the conflict markers.

Review the changes and decide which version should remain.

Developers can:

- Keep changes from the current branch.
- Keep changes from the incoming branch.
- Combine changes from both branches.

Remove the conflict markers and save the resolved files.

### Step 3: Stage the Resolved Files

Once the conflicts have been resolved, stage the affected files using:

```bash
git add <filename>
```

For example:

```bash
git add Assets/Scripts/PlayerMovement.cs
```

Staging the file tells Git that its conflicts have been resolved.

### Step 4: Complete the Merge

After resolving and staging all conflicting files, complete the merge using:

```bash
git commit
```

Alternatively, use:

```bash
git merge --continue
```

This completes the interrupted merge once all conflicts have been resolved.

It is recommended to run `git status` first to confirm that no unresolved conflicts remain.

## Aborting a Merge

Sometimes a developer may decide not to proceed with a merge.

To cancel an ongoing merge, use:

```bash
git merge --abort
```

This attempts to restore the repository to its state before the merge began.

**Warning:** If uncommitted changes existed before the merge, Git may not always be able to restore them correctly. It is recommended to commit or stash important changes before merging.

## Merge Conflicts in Game Development

Merge conflicts are particularly important in game development, where programmers and artists often work on shared project files.

For example, in a Unity project:

- Two programmers may modify the same C# script.
- Multiple developers may make conflicting changes to the same scene.
- Artists may edit the same models, textures, or other binary assets.
- Changes to shared project configuration files may conflict.

Text-based files, such as C# scripts, can often be resolved by manually editing the conflicting lines.

Binary files, such as 3D models and textures, cannot always be merged automatically. Developers may need to choose which version to keep or coordinate their changes with teammates.

Git LFS provides file locking functionality that can help prevent simultaneous edits to shared binary assets.

## Tips for Avoiding Merge Conflicts

Although merge conflicts cannot always be prevented, teams can reduce their frequency through good collaboration practices.

- **Communicate:** Coordinate with teammates before modifying shared files.
- **Use Feature Branches:** Develop features or fixes in dedicated branches.
- **Synchronize Regularly:** Keep branches updated with changes made by other team members.
- **Commit Frequently:** Make small, meaningful commits to simplify reviewing changes.
- **Divide Responsibilities:** Avoid unnecessary simultaneous edits to the same files.

## Additional Resources

- [Pro Git - Basic Branching and Merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)
- [GitHub Docs - Resolving a Merge Conflict Using the Command Line](https://docs.github.com/en/pull-requests/how-tos/merge-and-close-pull-requests/resolving-a-merge-conflict-using-the-command-line)
- [GitHub Docs - Resolving a Merge Conflict on GitHub](https://docs.github.com/en/pull-requests/how-tos/merge-and-close-pull-requests/resolving-a-merge-conflict-on-github)
- [Git Documentation - git merge](https://git-scm.com/docs/git-merge)
