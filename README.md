# learn-git-remote
This is a repository for learning how to use Git.

## Git Command Cheatsheet
### Basic Setup
Initialize a new Git repository:
```git init```

Configure the user name and email address:
```
git config --global user.name "Your Name"  
git config --global user.email "youremail@example.com"
```

### Basic Workflow
Check the current status of the repository:
```
git status
```

Add files to the staging area:
```
git add <filename>  
git add .  # Add all modified files in the current directory
```

Commit changes to the repository:
```
git commit -m "Commit message"
```

View the history of commits:
```
git log  
git log --oneline  # Shorter format
```

### Branching and Merging
List all branches:
```
git branch  
git branch -a  # Include remote branches
```

Create a new branch:
```
git branch <branchname>  
git checkout -b <branchname>  # Create and switch to new branch
```

Switch to an existing branch:
```
git checkout <branchname>  
git switch <branchname>  # Git 2.23+
```

Merge a branch into the current branch:
```
git merge <branchname>
```

Delete a branch:
```
git branch -d <branchname>  
git branch -D <branchname>  # Force delete
```

### Remote Repositories
List all remote repositories:
```
git remote -v
```
Add a new remote repository:
```
git remote add <remotename> <url>
```
Fetch from a remote repository:
```
git fetch <remotename>
```
Pull changes from a remote repository and merge into the current branch:
```
git pull <remotename> <branchname>  
git pull origin main  # Example
```
Push changes to a remote repository:
```
git push <remotename> <branchname>  
git push origin main  # Example
```

### fatal: refusing to merge unrelated histories
```
git pull origin main --allow-unrelated-histories
```
