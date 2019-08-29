# BHL Git and GitHub Training

Welcome to BHL Git and GitHub training! 

If you are new to Git and GitHub, or you need a refresher, you're in the right place. 

In this training, you will upload a python script to `bentley-historical-library/bhl_git_training` repository (repo) and learn how to:
- [Fork and clone a repository](https://github.com/bentley-historical-library/bhl_git_training#step-1-setting-up) 
- [Pull, commit, push changes](https://github.com/bentley-historical-library/bhl_git_training#step-2-understanding-workflow)
- [Create pull requests and resolve issues](https://github.com/bentley-historical-library/bhl_git_training#step-2-understanding-workflow)

## BEFORE YOU START
- For this training, you need to have Git on your computer and know basic terminal commands, such as `cd` and `ls`. This instruction was written for Git Bash on Windows.
  - See [this video](https://learning.oreilly.com/videos/learn-python-the/9780134686011/9780134686011-CLICCWindows) or [this book](https://learning.oreilly.com/library/view/learn-python-the/9780133124316/app03.html) (use your UofM ID for the login) if you need a crash course on terminal commands. 
- You can get your to-do list for this training by creating a new issue using the To-do List template.
  - Click Issues menu in the top-left; Then, click New issues button on the right side.
- This document includes common Git commands with a brief description of how it is used and what it does. You can learn more about each command by following `>> More` links.

## STEP 1. SETTING UP
### `git config`
```
git config --global user.name "YOUR NAME"
git config --global user.email YOUR@EMAIL
``` 
- Git uses a username to associate commits with an identity. [>> More](http://swcarpentry.github.io/git-novice/02-setup/index.html)
- Tip: 
  - To view your git settings, type `git config --list`

### Forking a repo
```
Click the Fork button in the top-right corner of a GitHub repo page
```
- A fork is a copy of a repo. Forking a repo allows you to freely experiment with changes without affecting the original project. [>> More](https://help.github.com/en/articles/fork-a-repo)

### `git clone`
```
git clone <repo_url> <directory>
```
- The `git clone` command copies a remote repo (e.g., a GitHub repo) to create a local copy on your computer. [>> More](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone)

### `git remote`
```
git remote add upstream <repo_url>
```
- The `git remote` command sets connections (i.e., bookmarks) to other repositories. [>> More](https://www.atlassian.com/git/tutorials/syncing)
- Tip:
  - To view your remote repositories, type `git remote -v`

## STEP 2. UNDERSTANDING WORKFLOW
### `git fetch`
```
git fetch upstream
```
- The `git fetch` command downloads commits, files, and refs from a remote repo into your local repo. It allows you to see what everybody else has been working on. [>> More](https://www.atlassian.com/git/tutorials/syncing/git-fetch)

### `git pull`
```
git pull upstream master
```
- The `git pull` command is used to fetch and download content from a remote repo and immediately update the local repo to match that content. [>> More](https://www.atlassian.com/git/tutorials/syncing/git-pull)

### `git add`
```
git add <file or directory>
```
- The `git add` command adds a change in the working directory to the staging area. It tells Git that you want to include updates to a particular file in the next commit. [>> More](https://www.atlassian.com/git/tutorials/saving-changes)

### `git commit`
```
git commit -m "commit message"
```
- Commits can be thought of as snapshots along the timeline of a project. Commits are created with the `git commit` command to capture the state of a project at that point in time. [>> More](https://www.atlassian.com/git/tutorials/saving-changes/git-commit)
- Tip:
  - Use the imperative mood for your commit message

### `git push`
```
git push
```
- The `git push` command is used to upload local repo content to a remote repo. Pushing is how you transfer commits from your local repo to a remote repo. [>> More](https://www.atlassian.com/git/tutorials/syncing/git-push)

## STEP 3. COLLABORATING 
### Creating Pull Requests and Resolving Issues
- What are pull requests? 
  - Pull requests let you tell others about changes you have pushed to a repo on GitHub. Once the request is reviewed and approved, your changes are merged into the repo. [>> More](https://help.github.com/en/articles/about-pull-requests)
- Using a pull request, you can resolve issues as well. In the body of your pull request, use GitHub syntax: close / fix / resolve + issue number (e.g., `Fixes #123`). [>> More](https://help.github.com/en/articles/closing-issues-using-keywords)

## BEFORE YOU LEAVE
That was the Git and GitHub basics! Before you leave, there are few *useful* things you might want to know:

### First and Foremost
```
When you are working with Git and GitHub, NEVER put confidential/senstive information (e.g., password, API keys, and etc.) into a repo.
```

### `.gitignore`
- A `.gitignore` file can be used to specify files and directories that should not be tracked by git. These might include log files, test data, configuration files created by a code editor, and so on.
- Files and directories to ignore can be specified by exact name (e.g., a directory named "test-data/" or a file called "secrets.txt") to ignore those specifics files or directories or by using a wildcard to ignore patters of files or directories (e.g., "*.log" to ignore all log files).
- [Learn more about .gitignore](http://swcarpentry.github.io/git-novice/06-ignore/index.html)

### `git status` and `git log`
```
git status
```
- The `git status` can be used to show which branch you are on, which files have uncommitted changes, whether or not your local repository is up-to-date with a remote repository, and so on.

```
git log
```
- The `git log` command can be used to list the commit history for your current branch or a specific file. Use `git log` to show all commits for the given branch and `git log filename` to show history for a specific file. [>> More about exploring your git history](http://swcarpentry.github.io/git-novice/05-history/index.html)

### Branching and Merging
```
git branch
```
- A git branch can be used to track a series of similar commits separate from the `master` branch. Branching is useful when you will be working on a specific feature request or issue that might require multiple commits or when working on multiple separate features at once to avoid committing too many conflicting changes to master. Use `git branch` to list all branches on your repository, `git branch [branch-name]` to create a new branch, and `git checkout [branch-name]` to switch to a specified branch.

```
git merge
```
- The `git merge` command can be used to combine (merge) the commits from a specified branch into your current branch. `git merge` will also report on conflicts that exist between the two branches, which will need to be resolved before the two branches can be combined. [>> More on branching and merging](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging)

## ADDITIONAL RESOURCE
- https://software-carpentry.org/lessons/
- https://guides.github.com/introduction/git-handbook
- https://www.atlassian.com/git/tutorials/
- https://realpython.com/python-git-github-intro/
- https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet

## ACKNOWLEDGMENTS
- This training resource was inspired by the GitHub Pages training, and each git command descriptions are from [GitHub Help](https://help.github.com), [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials), and [Software Carpentry](https://software-carpentry.org/lessons/index.html).