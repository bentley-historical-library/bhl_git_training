# BHL Git and GitHub Training

## 1. SETTING UP
### `git config`
- Open Git Bash and type:
```
git config --global user.name "YOUR_NAME"
git config --global user.email YOUR@EMAIL
``` 
---
- "Git uses a username to associate commits with an identity."
- Tip: 
  - To view your git settings, type `git config --list`

### Forking a repository
- On GitHub, click the Fork button in the top-right corner of the page
---
- "A fork is a copy of a repository."

### `git clone`
- Open Git Bash and type:
```
git clone <repo_url>
```
---
- The git clone command copies a remote repository (e.g., a repository on GitHub) to create a local copy on your computer.

### `git remote`
- Open Git Bash and type:
```
git remote add upstream <repo_url>
```
---
- The git remote command sets connections (i.e., bookmarks) to other repositories.
- Tip:
  - To view your remote repositories, type `git remote -v`

## 2. WORKFLOW
### `git fetch`
- Open Git Bash and type:
```
git fetch upstream
```
---
- "The git fetch command downloads commits, files, and refs from a remote repository into your local repository." It allows you to see what everybody else has been working on. 

### `git pull`
- Open Git Bash and type:
```
git pull upstream master
```
---
- "The git pull command is used to fetch and download content from a remote repository and immediately update the local repository to match that content."

### `git add`

### `git commit`

### `git push`
- Open Git Bash and type:
```
git push
```
---
- "The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo."

### Creating Pull Requests and Resolving Issues
- 

## 3. TBA

---
## ADDITIONAL RESOURCE
- https://software-carpentry.org/lessons/
- https://www.youtube.com/user/GitHubGuides/videos
- https://www.atlassian.com/git/tutorials/setting-up-a-repository
- https://guides.github.com/introduction/git-handbook
