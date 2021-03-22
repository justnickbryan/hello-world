# hello-world
My first foray into GitHub

## Introduction
I'm a newcomer to programming, data science and open-source, having previously studied and worked in neuroscience and pharma.
I'm taking one small step on my own journey, and a giant leap into the unknown world of github.
Learning Python for data science. I will be uploading personal projects and University assignments to this GitHub.

***

## Practicing for collaboration from the command line (Git Bash)

### Showing remote server

To show current configured remote servers:

```bash
git remote -v
```

Output:

```
origin  https://github.com/justnickbryan/hello-world.git (fetch)
origin  https://github.com/justnickbryan/hello-world.git (push)
```

If there was another collaborator working on the repo remotely and I had added that remote server, this might show:

```
origin  https://github.com/justnickbryan/hello-world.git (fetch)
origin  https://github.com/justnickbryan/hello-world.git (push)
<userID>  https://github.com/<userID>/hello-world.git (fetch)
<userID>  https://github.com/<userID>/hello-world.git (push)
```

### Pushing to remote

To push commits to remote server:

```bash
git push <remote> <branch>
```

So for my repo, in which there is only me working on a single remote with only the default main branch that would be:

```bash
git push origin main
```

### Creating & switching to a new branch

To create a new branch:

```bash
git branch <newBranchName>
```

For this commit, I'll create a new branch called 'practice':

```bash
git branch practice
```

Then to switch to the new 'practice' branch, use the checkout command (moves HEAD to point to practice branch):

```bash
git checkout practice
```

Output:

```
Switched to branch 'practice'
M       README.md
```

Note: it's possible to create a new branch and switch to it with a single command:

```bash
git checkout -b <newBranchName>
```

### Commit and push to new branch

```bash
git add .
git commit -m "add README.md updates regarding practice with branches"
git push origin practice
```
