---
title: Stashing
layout: default
nav_order: 6
---

# Stashing Changes: The Magic Toy Box

Git stash allows you to put aside changes that you don't want to commit immediately

![ToyBox](https://unsplash.com/photos/qBrF1yu5Wys)

Imagine a magic toy box:
- Allows kid to instantly clean their room
- When they want to play again, all toys are restored to their former positions


## When to Stash?

- You want to switch branches, but you're in the middle of something and don't want
to commit yet.
- You need to pull changes, but you have uncommitted work.


## Stashing in Action

`git stash`
This command stashes your changes, leaving you with a clean working directory.

**Remember, it's only a temporary storage. Don't forget about your stashed changes!**

## The Stash Stack

Think of 'git stash' as creating a stack of saved changes.
![StackOfPancakes](https://unsplash.com/photos/EIJD83grkK0)

You can stash multiple sets of changes and Git will store them in a LIFO (Last In, First Out) stack.

## Restoring Stashed Changes

To restore stashed changes, use:

- `git stash pop` - Re-applies the changes and removes them from the stash.
- `git stash apply` - Re-applies the changes but keeps them in the stash.

## Other Helpful Stash Commands

`git stash list`: Review all your stashes before deciding to apply or drop them.

`git stash drop`: Removes the most recent stash from the stack without applying it.

`git stash branch <branchname>`: Creates a new branch based on the popped stash.

`git stash clear`: This command removes all your stashes.

`git stash pop 'stash@{n}`: Pop a specific stash seen in `git stash list`.