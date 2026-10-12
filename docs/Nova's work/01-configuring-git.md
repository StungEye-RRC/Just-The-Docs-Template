---
title: Configuring Git
parent: Git Fundamentals
nav_order: 1
layout: default
---

# Configuring Git

Before you can start working with Git, you have to make sure it is fully set up and configured.

## Table of Contents
{: .no_toc}
1. TOC
{:toc}

## Install

First thing you will want to do is [install Git ands Git GUI] (https://gitforwindows.org/)

## Configuration

Next, launch Git Bash

You'll have to let Git know who you are by providing your name and email. You can do this with the following commands:
```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com
```

And for convenience, enable colourization.
```
git config --global color.ui auto
```

After these steps, your Git should be fully set up