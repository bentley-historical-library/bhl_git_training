# BHL Git and GitHub Training

## 1. SETTING UP
### `git config`
```
git config --global user.name "YOUR_NAME"
git config --global user.email YOUR@EMAIL
``` 
- "Git uses a username to associate commits with an identity."
- Tip: 
  - To view your git settings, type `git config --list`

### Forking a repository (repo)
```
Click the Fork button in the top-right corner of a GitHub repo page
```
- A fork is a copy of a repo.

### `git clone`
```
git clone <repo_url>
```
- The `git clone` command copies a remote repository (e.g., a GitHub repo) to create a local copy on your computer.

### `git remote`
```
git remote add upstream <repo_url>
```
- The `git remote` command sets connections (i.e., bookmarks) to other repositories.
- Tip:
  - To view your remote repositories, type `git remote -v`

## 2. WORKFLOW
### `git fetch`
```
git fetch upstream
```
- "The `git fetch` command downloads commits, files, and refs from a remote repository into your local repository." It allows you to see what everybody else has been working on. 

### `git pull`
```
git pull upstream master
```
- "The `git pull` command is used to fetch and download content from a remote repository and immediately update the local repository to match that content."

### `git add`
```
git add <file or directory>
```
- "The `git add` command adds a change in the working directory to the staging area. It tells Git that you want to include updates to a particular file in the next commit."

### `git commit`
```
git commit -m "commit message"
```
- "Commits can be thought of as snapshots along the timeline of a project. Commits are created with the `git commit` command to capture the state of a project at that point in time."
- Tip:
  - Use the imperative mood for your commit message

### `git push`
```
git push
```
- "The `git push` command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo."

### Creating Pull Requests and Resolving Issues

## 3. 
### `.gitignore`

### `git status` and `git log`

### Branching and Merging

### `git rebase`

---
## ADDITIONAL RESOURCE
- https://software-carpentry.org/lessons/
- https://guides.github.com/introduction/git-handbook
- https://www.youtube.com/user/GitHubGuides/videos
- https://www.atlassian.com/git/tutorials/setting-up-a-repository