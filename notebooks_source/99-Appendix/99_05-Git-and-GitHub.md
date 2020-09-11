---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: '0.9'
    jupytext_version: 1.5.0
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Git and GitHub

+++

**Git** is one of the standard _version control_ systems used by developers to save code and work on code collaboratively as a team. **Git** is a program run on the command line or **Anaconda Prompt**. If you use Windows, the **gitbash** program can be downloaded at [git-scm.com/downloads](https://git-scm.com/downloads). **Git** was created by Linus Torvalds, who also designed the Linux operating system.

+++

[GitHub.com](https://github.com/) (now owned by Microsoft) is a website and service used by programmers and open source projects to share code and allow contributors to propose changes to existing code. Other services such as [BitBucket.org](https://bitbucket.org) can be integrated with **git** too.

+++

Both **git** and [GitHub.com](https://github.com/) are useful for problem solvers working in teams.

+++

Before using **git** and GitHub.com, it is helpful to understand a couple of terms:

 * **git** - a command line program used to track file changes and collaborate on code with others.
 * **repo** - short name for "repository". A repo is a directory and its contents.
 * **local repo** -  a directory and its contents on your computer that **git** knows about.
 * **remote repo** - a directory and its contents stored in the cloud that **git** knows about.

+++

Useful **git** commands are summarized below:

 * ```git clone https://github.com/user/repo.git``` copy a remote repo from GitHub.com into a local directory
 
 * ```git init``` create a new local repo in the current folder
 
 * ```git remote add origin https://github.com/user/repo.git``` link a local repo to a remote repo on GitHub.com
 
 * ```git add .``` add all files and changes to the local repo
 
 * ```git commit -m "commit message"``` commit the changes in the local repo with the message ```"commit message"```
 
 * ```git push origin master``` push local changes up to the remote repo
 
 * ```git pull origin master``` pull down the version in the remote repo into the local repo

+++

## Cloning a repo

+++

One common operation to complete with **git** is to clone a repo from GitHub.com and save it locally. This means you copy all the files stored in the remote repo on GitHub.com onto your local computer. Cloning a repo from Github.com is accomplished with:

```text
$ git clone https://github.com/user/repo.git
```

This command copies the repo named ```repo``` from the user named ```user``` to a local computer. To clone the repo for MicroPython, use:

```text
$ git clone https://github.com/micropython/micropython.git
```

+++

## Creating and synching a remote repo on GitHub.com with a local repo

+++

Another common task to complete with **git** is to synch a remote repo on GitHub.com with a local repo on your local computer. This is useful when you want to keep the files in a particular project synched across multiple computers. Synched remote and local repos are also useful for a group of problem solvers working on the same project. Each team member has access to the same remote repo on GitHub.com and each team member has the same local repo on their computer.

### Create a remote repo on GitHub.com

First, go to [GitHub.com/join](https://github.com/join) and create a new account. Log in and create a new repo. It is a good idea to include a license and a **_.gitignore_** file. For a Python project, the **_.gitignore_** file for Python is a good start. Two common licenses for open source projects (projects you are willing to share with others) are the _GNU General Public License v3.0_ and the _MIT License_.

### Make a new local repo and link the local repo to the remote repo on GitHub.com

Second, create a local directory and ```cd``` into it. Initialize a git repo locally in that directory. Then synch the local folder with the remote repo on GitHub.com.

```text
$ mkdir newproject
$ cd newproject
$ git init
$ git remote add origin https://github.com/user/repo.git
$ git pull origin master
```

### Add, commit and push changes up to Github.com

Third, work on the project locally. For example, you could edit one of the files in the directory ```newproject``` or create a new file in the directory ```newproject```.

Finally, save your work and commit the changes you made with **git**. Push those changes up to the remote repo on GitHub.com

```text
$ git add .
$ git commit -m "commit message"
$ git push origin master
```

### Pull the most recent version from GitHub.com before each work session

If using **git** and GitHub.com, remember to pull the most recent version of the repo down from GitHub.com before you make any changes locally. If changes are made locally before the version of the repo on GitHub.com is synched, the local repo and remote repo will be out of synch.

```text
$ git pull origin master
```

After local changes are made, save the changes and push to GitHub.com

```text
$ git add .
$ git commit -m "commit message"
$ git push orign master
```

```{code-cell} ipython3

```
