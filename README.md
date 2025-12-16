# GitAndGithubIntro

Click the following link to view this website:<br/>
<a href="https://raza023.github.io/GitAndGithubIntro/">https://raza023.github.io/GitAndGithubIntro/</a>

# 🐙 Git Cheatsheet – All Commands with Descriptions

## 🛠 Initialize & Clone

- `git init` → Initialize a new local Git repository
- `git clone <url>` → Clone a remote repository to your local machine

## ✏️ Stage & Commit

- `git add <file>` → Stage a single file
- `git add .` → Stage all changes in the current directory
- `git reset <file>` → Unstage a staged file
- `git commit -m "message"` → Commit staged changes with a message
- `git commit -am "message"` → Stage and commit tracked files in one step
- `git commit --amend` → Modify the last commit

## 🔄 Push, Pull & Fetch

- `git push` → Upload local commits to the default remote branch
- `git push origin <branch>` → Push a specific branch to remote
- `git push -u origin <branch>` → Set default upstream branch & push
- `git push --force` → Force-push changes (use carefully)
- `git pull` → Download and merge changes from the remote
- `git pull --rebase` → Rebase local commits on top of remote changes
- `git fetch` → Download objects and refs without merging
- `git fetch --all` → Fetch all remotes

## 🌱 Branching

- `git branch` → List local branches
- `git branch -a` → List local and remote branches
- `git branch -r` → List remote branches
- `git branch <branch>` → Create a new branch
- `git branch -d <branch>` → Delete a local branch safely
- `git branch -D <branch>` → Force delete a local branch
- `git checkout <branch>` → Switch to a branch
- `git checkout -b <branch>` → Create and switch to a new branch
- `git checkout -b <new-branch> origin/<remote-branch>` → Create local tracking branch
- `git switch <branch>` → Switch branches (newer alternative)
- `git switch -c <branch>` → Create and switch to new branch
- `git merge <branch>` → Merge another branch into the current branch
- `git rebase <branch>` → Reapply commits on top of another base branch

## ✅ Stash & Patch

- `git stash` → Temporarily save changes
- `git stash push --staged -m "Message to stash only staged changes"` → Stash only staged changes
- `git stash pop` → Apply and remove the last stash
- `git stash list` → List saved stashes
- `git stash apply stash@{n}` → Apply a specific stash
- `git stash drop stash@{n}` → Delete a specific stash
- `git format-patch <commit>` → Create patch files from commits
- `git apply <patch>` → Apply patch file

## 📜 Logs & History

- `git log` → View full commit history
- `git log --oneline` → Compact single-line history
- `git log --graph --all --decorate` → Visual graph of branches and commits
- `git show <commit>` → Display details of a specific commit
- `git shortlog` → Summarized commit history
- `git reflog` → Show local branch history, including changes to HEAD

## 🔧 Reset, Revert & Fix

- `git reset <file>` → Unstage file without changing its content
- `git reset --soft <commit>` → Reset HEAD to commit, keep staged changes
- `git reset --mixed <commit>` → Reset HEAD and unstage changes
- `git reset --hard <commit>` → Reset HEAD and working directory to commit
- `git revert <commit>` → Create a new commit that undoes the specified commit
- `git cherry-pick <commit>` → Apply a commit from another branch

## 🔍 Inspect & Compare

- `git status` → Show current branch and staged/unstaged changes
- `git diff` → Show unstaged differences
- `git diff --staged` → Show staged differences
- `git diff <branch1>..<branch2>` → Compare two branches
- `git blame <file>` → Show last modification for each line
- `git bisect start / bad / good` → Find commit that introduced a bug

## 🌐 Remote

- `git remote -v` → List remote repositories
- `git remote add origin <url>` → Add a new remote named origin
- `git remote remove origin` → Remove the remote named origin
- `git remote rename <old> <new>` → Rename a remote
- `git remote set-url origin <new-url>` → Change remote URL

## ⚙️ Config & Setup

- `git config --global user.name "Name"` → Set global username
- `git config --global user.email "email@example.com"` → Set global email
- `git config --global core.editor "vim"` → Set default text editor
- `git config --list` → Show all current configurations

## 🧹 Clean & Maintenance

- `git clean -n` → Preview which untracked files would be removed
- `git clean -f` → Remove untracked files
- `git clean -fd` → Remove untracked files and directories
- `git gc` → Optimize the local repository
- `git fsck` → Check repository for integrity

## 📦 Tags & Releases

- `git tag` → List tags
- `git tag <name>` → Create a new lightweight tag
- `git tag -a <name> -m "message"` → Create an annotated tag
- `git tag -d <name>` → Delete a local tag
- `git push origin <tag>` → Push a single tag to remote
- `git push origin --tags` → Push all tags to remote
- `git fetch --tags` → Fetch tags from remote

## 📂 Submodules & Other

- `git submodule add <url> <path>` → Add new submodule
- `git submodule init` → Initialize local submodule config
- `git submodule update` → Fetch and checkout submodule
- `git archive --format zip --output=../archive.zip master` → Archive repository to zip

---

This cheatsheet now lists **commands with clear descriptions**



# Notes
----------------Some useful cmd commands----------------

---------for linux-------
01) pwd (print working directory)
02) ls (list contents of current directory)
03) ls -a (list contents including of current directory)
04) cd (change directory: used for navigaion b/w directories and folders)
05) cd .. (to go to previous directory)
06) cd /  (Root directory)
07) cd Downloads (to go to Downloads from Root directory)
08) cp file.txt filecopy.txt (copy file) [cp fileNameOfFileToCopy NameOfCopiedFile]
09) cp file.txt /home/hassan/Downloads   (copy file to Downloads folder)
10) rm file.txt (remove or delete file)
11) mkdir folder1 folder2 (make one or more directory)
12) rmdir folder1 (remove directory (only empty folder))
13) rm -r folder2 (to delete non-empty folder)
14) man ls (to see the details of command ls)
15) clear (clear screen)
16) touch f1.txt f2.txt (touch command is used to create one or more text files at a time in current working directory)
17) cat > file.txt (create and edit file)
18) cat file.txt (show file content)

---------for windows-------
01) mkdir folderName   (creates folder named as folderName)
02) cd ..   (change directory).
03) dir  (show files in directory)
04) cls (clear screen)

-------------------git commands-----------------

0) git --version       (to see git installed or not)
1) git init            (initiaize a git repository)
2) git status          (to see changes)
3) git add .           (git add f1.html (to add single file to staging area.))
4) git commit -m "your message goes here."
5) git log             (shows commits history)
6) git diff f1.txt     (shows differnce from last commit)
7) git checkout f1.txt (removes modification not addition)

reverting to old commit

8) git reset --hard  41192d2d0ec3e094a46b81c32c035859f7ee7da9 (bash number to which we have reverted just now)
9) git reset --soft HEAD@{1}
10)git add . 
11)git commit -m "reverted to old commit with bash 41192d2d0ec3e094a46b81c32c035859f7ee7da9"

local to remote repository(github)

12) git remote add origin https://github.com/accountName/repoName.git
13) git push -u origin master   (for all commits)
14) make changes now (locally)
15) git add .
16) git commit -m "new commit but its not on github"
17) git push -f origin master

Branching

1) git branch               (to see available branches)
2) git branch feature1      (creates branch named as feature1)
3) git checkout feature1    (switches the branch to feature1)
4) git merge feature1       (to merge branch named feature1 with the one you are currently on.)
4) git branch -d feature1   (deletes feature1 branch after merging)
5) git branch -D feature1   (deletes feature1 branch without merging)

fork, clone and pull request
1) git clone link clonedrepo
2) git remote add origin_clone link
3) git push -u origin_clone master

