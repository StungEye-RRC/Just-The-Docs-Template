---
title: Git Fundamentals
layout: default
nav_order: 3
---

# Git Fundamentals

## Configuring Git

First you need to tell Git who you are. Git needs your name and email. To do this you write these commands:
**git config --global user.name "Your Name"**
**git config --global user.email "your.email@example.com"**

You can also turn on somen helpful colourization if you want!
**git config --global color.ui auto**

You only need to set these one time. 

## Initializing a Repo 

To initialize a repo from the comman line you will type **git init .** inside the projects root folder. (Which means the command line should show the name of your projects folder before the >)

## Staging and Commiting Files

### Staging 

When we make changes to files in our repo we need to commit the changes, however before we can make a commit we must add new or changed files to a staging area. 

To stage the file you use the command **git add fileName.extension**  you can also use this command to add wildcards or sub-fodlers
or you can also use **git add .** to commit all new or modified files.

### Commiting

Now we can commit our changes to the repo. To do this we use this **git commit** command. When commiting we also must attach a message. Using the previous command will open a text editor for you to write your message. You can also do this in the command line by using **git commit -m "Your commit message"** 

If your change requires it you can also add a title by adding another **-m "Title"** before your commit message.

**_Good commit messages are crucial. They allow for: traceability, collabaoration, documentation, and change management._**

## Status, Log, and Diff

### Checking Your Repo's Status

You can check the status of your repositiory by using **git status** this will show changes or additions in your repository.

### Git Log

You can review your commits by using **git log**. Log enteries show: the commit hash, who made the commit, when the commit was made, and the commit message.

### Git Diff

To compare and see the changes from current files and the latest commit you can use **git diff**, this command will show all the differences in the repo. If you want to see the diff of a specific file you can add the file name and extension **git diff fileName.extension**. Or you can view a specific folder by putting the folder location in **git diff ./myFile**

## Git Ignore File

Sometimes you have files in your project that you don't want to include in your repo. Some examples of this are: files that include passwrods or API keys (or other secrets), temporary files and folders, build files and folders, Hidden OS files.

To do this you can create a .gitignore file in your project root. 

In your .gitignore file you can ignore specific files by writing **fileToIgnore.txt**

Or you can ignore all files with a specific extension ***.exe** (this will ignore all .exe files). If there's a file with your ignore extension that you **_do_** want to track you can write **!special.a** 

You can also ignore all files in a specific folder **ignoreFolder/**

Or you can ignore specific files in a specific folder **ignoreFolder/****/*.pdf** (this will ignore all .pdf files in the ignoreFolder).


