---
title: Git Revert
parent: Undoing in Git
nav_order: 3
---

# When to Use Revert?

Use `git revert` to run a specific commit **in reverse.**

Typically used to undo a commit that has been shared with others.

*The public undo - it says, 'I made a mistake, but I want to keep a record of it.'*

## Reverting Commits

`git revert <commit id>`

Creates a new commit that undoes changes from the specified commit.

**The Safest Undo Choice!**

Reverting maintains history, making it a safe choice for:

- Undoing local commits.

- Undoing commits pushed to a remote repo.

### Before Revert: HEAD at D

![Before Revert, Head at D](https://i.imgur.com/YRVmxmG.png)

If we wish to revert the changes made in D:

`git revert D`

### After Revert: HEAD at E

![After Revert, Head at E](https://i.imgur.com/sqZmCOE.png)

## Reverting Multiple Commits

The `git revert` command reverts a single commit by default.

We can run it multiple times to revert multiple commits:

```bash
git revert D
git revert C
```

Or we can revert a sequence of commits: *(Each commit is reverted separately!)*

```bash
git revert C^..D
```

If you only want a single revert commit: *(The `-n` stands for "no commit".)*

```bash
git revert D
git revert C
```