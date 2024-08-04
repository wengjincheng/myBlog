---
title: Git Usage
published: 2024-08-04
description: 'List the common git usage'
image: ''
tags: ['Git']
category: 'Git'
draft: false 
---

## create new branch

``` shell
git checkout -b branchname
```

## revoke operations

``` shell
git checkout -f // revoke all uncommit changes, but do delete these changes

git reset --soft HEAD^ // revoke latest commit, kepp changes but in stagging space

git reset --mixed HEAD^ // revoke latest commit and add, kepp changes (default)

git reset --hard HEAD^ // revoke latest commit and add. do not keep changes
```

## check local and remote branch


``` shell
git branch // local

git branch -r // remote
```

## rename local branch

``` shell
git branch -m oldname newname
```

## delete local/remote branch

``` shell
git branch -d branchname // local

git push origin --delete branchname // remote
```

## update remote branch list
``` shell
git remote update origin --prune
```

## check&change commit

``` shell
git log // check

git commit --amend // change latest commit
```

## discard commits

``` shell
git reset --hard commitname // 这个commit之后的commits都会被删除
```

## Tags

``` shell
git tag // check local tag

git tag <tagname> // create tag

git push origin <tagname> // push tag to remote
```

### refers

- https://www.cnblogs.com/lfxiao/p/9378763.html
- https://git-scm.com/docs/git-reset


