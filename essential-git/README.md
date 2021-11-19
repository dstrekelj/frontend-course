# Frontend Course / Essential Git

[:arrow_backward: Frontend Course](../README.md)

---

## Day 1

Version control systems (VCS) manage changes made to data.

You have probably already used a VCS without knowing. Word processors such as Microsoft Word, for example, use a type of VCS to track the history of changes made to the document.

Similarly, in the world of software development VCS track changes made to the _files_ of a software project, rather than just changes to a _single file_ (although they can do that too). These changes are tracked in a database called a repository, where every stored change is called a commit.

A VCS can be either centralised or distributed. Centralised VCS host the repository on a server that client computers connect to it in order to push and pull changes from the repository. Distributed VCS opt for every computer to have its own copy of the repository that the computers synchronise between themselves in a network of peers.

The peer-to-peer approach of a distributed VCS means users can work offline, privately, and not worry about losing data since backups are a positive side-effect of everyone having a copy of the repository. However, distributed VCS also require more storage space on the user's computer and may pose a security risk due to code base exposure - again, a side effect of everyone having a copy of the repository.

Our VCS of choice will be Git - a free, open source, and widely available distributed VCS. Although others exist (such as Subversion and Mercurial), Git has become the de facto standard for the software industry.

From this point on, we will discuss version control as it is handled by Git. Terminology and implementation details may differ between different VCS, but the general idea is roughly the same.

A Git **repository** stores commits in a tree-like fashion where every commit belongs to a **branch**. To continue the tree-like analogy, the trunk of the tree is commonly called the **master branch** - the "masterwork" or latest (usually stable) state of the project.

@todo tracked, untracked files

A **commit** contains one or more changes made to tracked files, along with a bundle of useful information: the author of the change; the time and date of the change; a unique hash ID of the change; and more.

Every commmit represents a snapshot of a state in which the repository was recorded to be at a set point in time. The commit that represents the currently observed repository state is called the **HEAD** commit.

@todo "checking out"

The commit history of a repository might look like this:

```
* 214291a (HEAD -> master) Add index and images
* 36e9ad7 Add README file
* 80c7f54 Initial commit
```

Initialise a Git repository with

```sh
git init
```

```sh
git status
```

## Day 2

```sh
git add
```

```sh
git reset
```

```sh
git diff
```

```sh
git commit
```

```sh
git rm
```

```sh
git logo
```

## Day 3

```sh
.gitignore
```

```sh
.gitkeep
```