---
title: Remove a file from the last commit
type: snippet
language: git
tags: [commit]
author: chalarangelo
cover: cancel-typographer
dateModified: 2021-04-13
---

Removes a file from the last commit without changing its message.

- Use `git rm --cached <file>` to remove the specified `<file>` from the index.
- Use `git commit --amend` to update the contents of the last commit, without changing its message.

```shell
git rm --cached <file>
git commit --amend
```

```shell
git rm --cached "30-seconds.txt"
git commit --amend
# Removes `30-seconds.txt` from the last commit
```
