# Lab - Git

## Description

This is an individual lab in a group. You do the labs on your local machine and help each other.

## Prerequisites

git

## Objectives

- Basic git commands

## Software

git

## TODO

### Basic git

#### Create an empty repository and make an initial commit

- Create an empty repository

- Check status

- Create a new file and save

- Check status

- Add file to the index

- Check status

- Make an initial commit

#### Checkout to a new branch, make changes and merge it back to master

- Checkout a new branch and with a name of choice

- Create two new files, both with content and save

- Check status

- Add file to the index

- Check status

- Make a commit

- Make a change in the content of both of the file and save

- Show changes between commits

- Add file to the index

- Check status

- Make a commit

#### Merge branch to master

- Check status and verify that there are nothing to be commited

- Check branches merged in master

- Checkout to master branch

- Verify that you have master and another branch

- Verify that you only have the initial file

- Merge branch into master

- Verify that you have merged

### Basic git commands (hints)

```bash
git init
git status
git commit
git checkout
git add
git diff
git branch
git merge
git help
```
---

### Answers

#### Create an empty repository and make an initial commit

- Create an empty repository

```bash
git init
```

- Check status

```bash
git status
```

- Create a new file and save

```bash
touch file-1.txt
```

- Check status

```bash
git status
```

- Add file to the index

```bash
git add file-1.txt
```

- Check status

```bash
git status
```

- Make an initial commit

```bash
git commit -m "Init"
```

#### Checkout to a new branch, make changes and merge it back to master

- Checkout a new branch and with a name of choice

```bash
git checkout -b my-new-branch
```

- Create two new files, both with content and save

```bash
echo "My content" > "file-2.txt"
echo "My content again" > "file-3.txt"
```

- Check status

```bash
git status
```

- Add file to the index

```bash
git add .
```

- Check status

```bash
git status
```

- Make a commit

```bash
git commit -m "Added two files"
```

- Make a change in the content of both of the file and save

```bash
echo "More of my content" > "file-2.txt"
echo "More of my content again" > "file-3.txt"
```

- Show changes between commits

```bash
git status
```

- Add file to the index

```bash
git add .
```

- Check status

```bash
git status
```

- Make a commit

```bash
git commit -m "Added changes"
```

#### Merge branch to master

- Check status and verify that there are nothing to be commited

```bash
git status
```

- Check branches merged in master

```bash
git branch --merged master
```

- Checkout to master branch

```bash
git checkout master
```

- Verify that you have master and another branch

```bash
git branch
```

- Verify that you only have the initial file

```bash
ls
```

- Merge branch into master

```bash
git merge my-new-branch
```

- Verify that you have merged

```bash
git branch --merged master
```