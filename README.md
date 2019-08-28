# BHL Git and GitHub Training

Welcome to BHL Git and GitHub training! 

If you are new to Git and GitHub, or you need a refresher, you're in the right place. 

In this training, you will upload a python script to `bentley-historical-library/bhl_git_training` repository (repo) and learn how to:
- [Fork and clone a repository]() 
- [Pull, commit, push changes]()
- [Create pull requests and resolve issues]()

## BEFORE YOU START
- For this training, you need to have Git on your computer and know basic terminal commands, such as `cd` and `ls`. This instruction was written for Git Bash on Windows.
- You can get your to-do list for this training by creating a new issue using the To-do List template.
  - Click Issues menu in the top-left; Then, click New issues button on the right side.
- This README.me includes common Git commands with a brief description of how it is used and what it does. You can learn more about each command by following `>> More` links.

## STEP 1. SETTING UP
### `git config`
```
git config --global user.name "YOUR NAME"
git config --global user.email YOUR@EMAIL
``` 
- Git uses a username to associate commits with an identity. [>> More](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-config)
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

### `.gitignore`

### `git status` and `git log`

### Branching and Merging

### `git rebase`

---
## ADDITIONAL RESOURCE
- https://software-carpentry.org/lessons/
- https://guides.github.com/introduction/git-handbook
- https://www.atlassian.com/git/tutorials/
- https://www.youtube.com/user/GitHubGuides/videos
- https://realpython.com/python-git-github-intro/

## ACKNOWLEDGMENTS
- This training resource was inspired by the GitHub Pages training, and each git command descriptions are from [GitHub Help](https://help.github.com) and [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)