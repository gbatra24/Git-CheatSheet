# Git-CheatSheet
Git-CheatSheet is a repository to quickly access commonly used commands in git.

### Create
1. Clone an existing repository
```bash
git clone <repo-url>
```

2. Create a new local repository
```bash
git init
```

### Local Changes
1. View changed files in your working directory
```bash
git status
```

2. View changes to tracked files
```bash
git diff
```

3. Add all current changes to the next commit
```bash
git add .
```

4. Add some changes in <file> to the next commit
```bash
git add -p <file>
```
  
5. Commit all local changes in tracked files
```bash
git commit -a
``` 

6. Commit previously staged changes
```bash
git commit
```

7. Change the last commit
```bash
git commit --amend
```

### Commit History
1. Show all commits
```bash
git log
```

2. Show changes over time for a specific file
```bash
git log -p <file>
```

3. Who changed what and when in <file>
```bash
git blame <file>
```
  
### Branches and Tags
1. List all existing branches
```bash
git branch -av
```

2. Switch HEAD branch
```bash
git checkout <branch>
```

3. Create a new branch based on your current HEAD
```bash
git branch <new-branch>
```

4. Create a new tracking branch based ona remote branch
```bash
git checkout --track <remote/branch>
```

5. Delete a local branch
```bash
git branch -d <branch>
```

6. Forceful delete a branch
```bash
git branch -D <branch>
```

7. Mark the current commit with a tag
```bash
git tag <tag-name>
```

### Update and Publish
1. List all currently configured remotes
```bash
git remote -v
```

2. Show information about a remote
```bash
git remote show <remote>
```

3. Add new remote repository, named <remote>
```bash
git remote add <shortname> <url>
```
  
4. Download all changes from <remote>, but don‘t integrate into HEAD
```bash
git fetch <remote>
```
  
5. Download changes and directly merge/integrate into HEAD
```bash
git pull <remote> <branch>
```

6. Publish local changes on a remote
```bash
git push <remote> <branch>
```

7. Delete a branch on the remote
```bash
git branch -dr <remote/branch>
```

8. Publish your tags
```bash
git push --tags
```

### Merge and Rebase
1. Merge <branch> into your current HEAD
```bash
git merge <branch>
```
  
2. Rebase your current HEAD onto <branch>
```bash
git rebase <branch>
```
  
3. Abort a rebase
```bash
git rebase --abort
```

4. Abort a merge
```bash
git merge --abort
```

5. Continue a rebase after resolving conflicts
```bash
git rebase --continue
```

6. Use your configured merge tool to solve conflicts
```bash
git mergetool
```

### Undo
1. Discard all local changes in your working directory
```bash
git reset --hard HEAD
```

2. Discard local changes in a specific file
```bash
git checkout HEAD <file>
```

3. Revert a commit (by producing a new commit with contrary changes)
```bash
git revert <commit>
```

4. Reset your HEAD pointer to a previous commit and discard all changes since then
```bash
git reset --hard <commit>
```

5. Reset your HEAD pointer to a previous commit and preserve all changes as unstaged changes
```bash
git reset <commit>
```

6. Reset your HEAD pointer to a previous commit and preserve uncommitted local changes
```bash
git reset --keep <commit>
```


  
  
