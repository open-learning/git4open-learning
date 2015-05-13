# `git4ol` Activities

At it's core a learning experience can be thought of as a guided set of activities a student takes to eventually get certified on a defined topic.

In `git4ol` we translate that experience to `git` commits and refs and the same way that `git` commits are the main building blocks of a `git` repository activities are the main building blocks of a `git4ol` lesson.

## Assets

Activity assets are located in directories according to this naming scheme:

- Step assets are located in directories of the format `refs/{lesson}@{version}/step/{n}` where
  - `lesson` is the name of the lesson
  - `version` is a valid semver
  - `n` is a positive number indicating the step number

- Challenge assets are located in directories of the format `refs/{lesson}@{version}/challenge/{challenge}` where
  - `lesson` is the name of the lesson
  - `version` is a valid semver
  - `challenge` is the name of the challenge

## Title and instructions

Activity title and instructions serialized with a combination of [front matter](http://jekyllrb.com/docs/frontmatter/) and [Markdown](http://daringfireball.net/projects/markdown/) (so basically [Jekyll](http://jekyllrb.com/)).

```
---
title: Our first markdown file
sha: 1158e62f02de11ddb51609a9efc8bebe655e1017
type: ide
files:
  - README.md
---

[Markdown](http://daringfireball.net/projects/markdown/) is a text-to-HTML conversion tool for web writers. Markdown allows you to write using an easy-to-read, easy-to-write plain text format

Let's start by adding a `README.md` file with some mock content.
```