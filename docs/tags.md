---
title: Tags
layout: default
nav_order: 8
---
<!-- prettier-ignore-start -->
# Tags
{: .no_toc }

Tags in Git act like bookmarks for important milestones in your project.
They can be used to mark release points (v1.0.0, v.1.1.0, etc).

## Table of Contents 
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Creating Tags
To create a new lightweight tag:
`git tag <tag-name>` or `git tag <tag-name> <commit hash>`
This will tag the current or specified commit with the provided name.

**tags should only include characters [a-z], [A-Z], numbers [0-9] or a dash/hyphen [-]**

## Annotated Tags
Annotated Tags store additional meta data such as taggers name, email, date, and an optional message.
`git tag -a <tag-name> -m "tag message"`

## Once You've Created a Tag
**Checkout to the tag:** You can tre a tag like a branch or a commit. and you can checkout to the tag's point in history. `git checkout <tag-name>`.

**List Tags:** You can list all the tags in the repo using `git tag` or `git tag -l`. To narrow a list based on a search pattern you can use `git tag -l "<search-pattern>"`.

**Show Tag Information:** If you have annotated tags, you can view the associated information with `git show <tag-name>`.

**Compare Differences:** If you can compare differences between the tagged state of code and the current HEAD using `git diff <tag-name>`.

## Additional Resources
[Git Tag documentation](https://git-scm.com/docs/git-tag)
[Git Hub Tags Page](https://docs.github.com/en/rest/git/tags?apiVersion=2022-11-28)