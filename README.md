# GitAndGithubIntro

Click the following link to view this website:<br/>
<a href="https://raza023.github.io/GitAndGithubIntro/">Click here</a>

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

12) git remote add origin https://github.com/Syed2958/gitpractice.git
13) git push -u origin master   (for all commits)
14) make changes now (locally)
15) git add .
16) git commit -m "new commit but its not on github"
17) git push -f origin master

Branching

1) git branch               (to see available branches)
2) git branch feature1      (creates branch named as feature1)
3) git checkout feature1    (switches the branch to feature1)
4) git merge feature1       (to merge branche named feature1 with the one you are currently on.)
4) git branch -d feature1   (deletes feature1 branch after merging)
5) git branch -D feature1   (deletes feature1 branch without merging)

fork, clone and pull request
1) git clone link clonedrepo
2) git remote add origin_clone link
3) git push -u origin_clone master

