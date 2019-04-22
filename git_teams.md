# Git For Teams

## Downloads

- [Git for Windows](https://gitforwindows.org/)
- [Git for MacOS](http://git-scm.com/download/mac)

---

## Terminology

#### Local Repository

> A git repository on our local system

#### Remote Repository

> A git repository hosted on a remote system (Github)

#### Stage

> Changes to be added to a repository

#### Commit

> Add changes to a repository

#### Merge

> Combine two branches in a repository

#### Stashe

> Temporary storage for changes

## Commands

#### Create a local git repository

```
git init
```

#### Pull a repository from github (clone)

```
git clone https://github.com/user/repo.git
```

#### Create a new branch

```
git checkout -b BRANCHNAME
```

#### Stage and commit changes to your local repository

```
git add .
git commit -m "message"
```

#### Push changes from local to remote

```
git push origin BRANCHNAME
```

#### Pull changes from remote to local

```
git pull
```

# Stashing

#### Stash changes

```
git stash
```

#### View stashes

```
git stash list
```

#### Apply stashed changes

```
git stash apply
```

#### Discard stash

```
git stash drop
```

# Merging

#### Checkout the destination branchB into branchA

```
git checkout branchA
```

#### Merge into the destination branch

```
git merge branchB
```

#### Pushed merged branch

```
git push origin branchA
```
