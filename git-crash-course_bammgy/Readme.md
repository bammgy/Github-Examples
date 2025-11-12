## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our project is a git repo.

If we want to create a git repo in a new project we create the folder and then initialize that repo using `git init`

```sh
mkdir /workspaces/temp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add .
# make changes to readme.md
git commit -m "add readme file"
```

## Cloning

We can clone three ways: HTTPS, SSH, GitHub CLI

Since we are using GitHub Codespaces we'll create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

## HTTPS

```sh
git clone https://github.com/bammgy/Github-Examples.git
cd GitHub-Examples
``` 

## Commits

When wa want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit
```

Set the global editor

```
git config --global core.editor emacs
```


## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage changes that will be included in the commit
We can use the . to add all possible files.

```
git add Readme.md
```

## Reset

Reset allows you move staged changes to be unstaged.
This is useful when you want to revert all files not to be commited.

```sh
git add. 
git reset

```

## Status

Git status shows you what files will or will not be commited.

```
git status
```
## Gitconfig

The gitconfig file is what stores your global configuration for git such as email, name, editor and more

Showing the contents of our .gitconfig file
```
git config --list
```

When you first install Git on a machine you are supposed to set up your name and email

```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```
