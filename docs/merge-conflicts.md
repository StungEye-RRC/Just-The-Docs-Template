---
title: Merge Conflicts
layout: default
nav_order: 6
---
<!-- prettier-ignore-start -->
# Merge Conflicts
{: .no_toc }

Merge conflicts occur when Git can't perform a fast-forward merge on two branches.
When a merge conflict happens, Git will alert you in the terminal and mark the areas of conflict in the file.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Git Markup
Git uses special markers to indicate the start and end of the confliced area:

`<<<<<<< HEAD` shows the start of the changes in the current branch.
`=======` shows the seperation between the changes in the current branch, and the merging branch.
`>>>>>>> branch-name` shows the end of the changes in the merging branch.

## Resolving Merge Conflicts
**How to resolve a merge conflict:**

- Edit the file to fix the conflicting changes. _Be sure to remove the conflict markers._
- Add the file to the staging area with `git add`.
- Commit the fix with `git commit`.

## Additional Resources

[Merge Conflicts](https://docs.gitlab.com/ee/user/project/merge_requests/conflicts.html)

[How to Resolve a Merge Conflict](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line)


