Первый опыт работы с GIT

""
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

PS C:\Users\t4555\OneDrive\Desktop\testGIT> git init
Initialized empty Git repository in C:/Users/t4555/OneDrive/Desktop/testGIT/.git/
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git add .
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   123.txt

PS C:\Users\t4555\OneDrive\Desktop\testGIT> git commit -m "first commit"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 't4555@��123.(none)')
PS C:\Users\t4555\OneDrive\Desktop\testGIT>   git config --global jgxxxz "t45552459@gmail.com"
error: key does not contain a section: jgxxxz
PS C:\Users\t4555\OneDrive\Desktop\testGIT>   git config --global t45552459 "t45552459@gmail.com"
error: key does not contain a section: t45552459
PS C:\Users\t4555\OneDrive\Desktop\testGIT>  git config --global user.email "you@example.com"
PS C:\Users\t4555\OneDrive\Desktop\testGIT>   git config --global user.name "Your Name"
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git commit -m "first commit"
[master (root-commit) aaa24cf] first commit
 1 file changed, 3 insertions(+)
 create mode 100644 123.txt
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git branch -M main
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git remote add origin https://github.com/jgxxxz/testGit.git
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 218 bytes | 72.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/jgxxxz/testGit.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   123.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        456..txt

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git add .
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   123.txt
        new file:   456..txt

PS C:\Users\t4555\OneDrive\Desktop\testGIT> git commit -m "second commit"
[main 4092363] second commit
 2 files changed, 8 insertions(+), 1 deletion(-)
 create mode 100644 456..txt
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 313 bytes | 156.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/jgxxxz/testGit.git
   aaa24cf..4092363  main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   123.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git add .
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git commit -m "3 commit"
[main 0e61e19] 3 commit
 1 file changed, 7 insertions(+), 1 deletion(-)
PS C:\Users\t4555\OneDrive\Desktop\testGIT> git push https://github.com/jgxxxz/testGit.git
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 281 bytes | 281.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/jgxxxz/testGit.git
   4092363..0e61e19  main -> main
PS C:\Users\t4555\OneDrive\Desktop\testGIT>



<img width="1758" height="839" alt="image" src="https://github.com/user-attachments/assets/fd8e047a-683a-44f4-ba23-c0c1d12f9ebe" />
