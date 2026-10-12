---
title: Learn Git Branching
layout: default
nav_order: 20
---

# Learn Git Branching
{: .no_toc }

## Overview

[Learn Git Branching](https://learngitbranching.js.org/) is a free, interactive website designed to help developers learn Git through visual tutorials and challenges.

Rather than simply reading about Git commands, users can enter commands into a simulated terminal and watch how they affect a visual representation of a repository.

The website is useful for both beginners and experienced developers looking to improve their understanding of Git.

## Table of Contents
{: .no_toc }

- TOC
{:toc}

## History and Creation

Learn Git Branching was created by software developer Peter Cottle, with its GitHub repository dating back to August 2012.

The project's main purpose is to help developers understand Git through visualization, something that can be difficult when working entirely through the command-line interface.

The website was developed using JavaScript and runs directly in a web browser.

Learn Git Branching is open source under the MIT License, allowing developers to view, modify, and contribute to its source code.

The project has also received contributions from the community, including translations, testing, and additional functionality.

## How Does Learn Git Branching Work?

Learn Git Branching simulates a Git repository inside the user's browser.

Users enter Git commands into a terminal, and a visual commit tree updates to show the effects of each command.

The website uses interactive tutorials and challenges to teach concepts such as:

- Creating commits and branches.
- Switching between branches.
- Merging and rebasing.
- Resetting and reverting changes.
- Working with remote repositories.
- Understanding Git's commit history.

The visualization makes it easier to understand how Git commands affect a project's history.

## Main Features

### Interactive Tutorials

Learn Git Branching includes a series of lessons that introduce Git concepts through progressively more challenging exercises.

Each level presents a specific objective that users must complete by entering Git commands.

The website provides visual feedback, allowing users to understand how their commands affect the repository.

### Sandbox Mode

Sandbox mode allows users to experiment with Git commands in a simulated repository without following a specific lesson.

This is useful for testing commands and understanding their effects without risking changes to a real project.

Users can also enter `undo` to reverse their previous simulated command or `reset` to restart the exercise.

### Visual Commit History

The website displays commits and branches using an interactive graph.

As users enter commands, the graph updates to represent changes to the repository's history.

This is particularly useful when learning about branching, merging, rebasing, and other operations that can be difficult to visualize through the terminal alone.

### Custom Levels

Learn Git Branching also allows users to create and share custom challenges using its level builder.

This makes it a useful resource for instructors, students, and developers who want to practice particular Git concepts.

## How to Get Started

1. Visit [Learn Git Branching](https://learngitbranching.js.org/).
2. Open the interactive lessons or enter `levels` in the simulated terminal.
3. Choose a lesson from the available challenges.
4. Read the objective and enter the required Git commands.
5. Watch the commit tree update as commands are executed.
6. Continue through the lessons or experiment independently in sandbox mode.

### Practical Example

Imagine a developer wants to learn how to create a new branch without affecting the main project.

Inside the Learn Git Branching terminal, they can enter:

```bash
git branch feature
```

This creates a new branch called `feature`.

They can then switch to it using:

```bash
git checkout feature
```

The website will update its visual commit tree to show the current branch.

Unlike practicing in an actual repository, the simulation allows developers to experiment without modifying real project files.

## Learn Git Branching in Game Development

Learn Git Branching is especially useful for game development programmers and artists who are new to version control.

Knowing about this tool can come in handy when there is somebody new to version control joining your team. Hand them this resource, and they can get up to speed on version control for _game_ development using a _game_!

For example, in a collaborative Unity project:

- Programmers can learn how to create branches for new game mechanics.
- Artists can better understand how their work fits into a team's version control workflow.
- Developers can visualize how different branches are merged together.
- Team members can practice undoing changes before using potentially destructive commands in a real project.

The website provides a safe environment for learning Git before applying these skills to larger game development projects.

**Note:** Learn Git Branching is a simulator and does not replace working with actual Git repositories. It is best used alongside practical experience with Git.

## Additional Resources

- [Learn Git Branching - Interactive Website](https://learngitbranching.js.org/)
- [Learn Git Branching - GitHub Repository](https://github.com/pcottle/learnGitBranching)
- [Learn Git Branching - All Levels Documentation](https://learngitbranching.js.org/generatedDocs/levels.html)
- [Learn Git Branching - MIT License](https://github.com/pcottle/learnGitBranching/blob/main/LICENSE.md)
