valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix
$ git init
Initialized empty Git repository in C:/Exam/Multi-Branch Feature Development and Hotfix/.git/

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ echo "Hello from main" > file.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git add .
warning: in the working copy of 'file.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git commit -m "Initial init commit"
[main (root-commit) 74f4647] Initial init commit
 1 file changed, 1 insertion(+)
 create mode 100644 file.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git checkout -b feature-auth
Switched to a new branch 'feature-auth'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ echo "Hello from feature-auth" > file1.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git add .
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git commit -m "first change in file1.txt"
[feature-auth 948e706] first change in file1.txt
 1 file changed, 1 insertion(+)
 create mode 100644 file1.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ echo "git log second commit" > file2.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git add .
warning: in the working copy of 'file2.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git commit -m "add info in file2.txt"
[feature-auth 4edd51a] add info in file2.txt
 1 file changed, 1 insertion(+)
 create mode 100644 file2.txt
 
valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ echo "Login interactive in github" > auth-login.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git add .
warning: in the working copy of 'auth-login.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git commit -m "Created new login auth-login.txt"
[feature-auth aa51e4e] Created new login auth-login.txt
 1 file changed, 1 insertion(+)
 create mode 100644 auth-login.txt
$ echo "git add new line!" > file3.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git add .
warning: in the working copy of 'file3.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git commit -m "added new file file3"
[feature-auth b18529e] added new file file3
 1 file changed, 1 insertion(+)
 create mode 100644 file3.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git status
On branch feature-auth
nothing to commit, working tree clean

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git log --oneline
b18529e (HEAD -> feature-auth) added new file file3
aa51e4e Created new login auth-login.txt
4edd51a add info in file2.txt
948e706 first change in file1.txt
74f4647 Initial init commit

git switch main
Switched to branch 'main'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git checkout -b feature-dashboard
Switched to a new branch 'feature-dashboard'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ echo "new dashboard view" > dashboard.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git add .
warning: in the working copy of 'dashboard.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git commit -m "added new dashboard.txt"
[feature-dashboard 7f7c827] added new dashboard.txt
 1 file changed, 1 insertion(+)
 create mode 100644 dashboard.txt

$ git switch main
Switched to branch 'main'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git checkout -b feature-dashboard
Switched to a new branch 'feature-dashboard'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ echo "new dashboard view" > dashboard.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git add .
warning: in the working copy of 'dashboard.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git commit -m "added new dashboard.txt"
[feature-dashboard 7f7c827] added new dashboard.txt
 1 file changed, 1 insertion(+)
 create mode 100644 dashboard.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ echo "update into new dashboard views" >> dashboard.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git add .
warning: in the working copy of 'dashboard.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git commit -m "update added for new dashboard.txt"
[feature-dashboard cd30c76] update added for new dashboard.txt
 1 file changed, 1 insertion(+)
 valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git switch main
Switched to branch 'main'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$  git checkout -b hotfix-security
Switched to a new branch 'hotfix-security'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (hotfix-security)
$ echo "this is a hot fix in security login" > secure-login.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (hotfix-security)
$ git add .
warning: in the working copy of 'secure-login.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (hotfix-security)
$ git commit -m "Fix bug in security login in secure-login.txt"
[hotfix-security fbf3749] Fix bug in security login in secure-login.txt
 1 file changed, 1 insertion(+)
 create mode 100644 secure-login.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (hotfix-security)
$ git switch main
Switched to branch 'main'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git merge hotfix-security
Updating 74f4647..fbf3749
Fast-forward
 secure-login.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 secure-login.txt
valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ echo "git add new line from feature-dashboard!" > file.txt

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git add .
warning: in the working copy of 'file.txt', LF will be replaced by CRLF the next time Git touches it

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git commit -m "updated new line in file"
[feature-dashboard 026b639] updated new line in file
 1 file changed, 1 insertion(+), 1 deletion(-)

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git switch feature-auth
Switched to branch 'feature-auth'
valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git status
On branch feature-auth
nothing to commit, working tree clean

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git log --oneline
b18529e (HEAD -> feature-auth) added new file file3
aa51e4e Created new login auth-login.txt
4edd51a add info in file2.txt
948e706 first change in file1.txt
74f4647 Initial init commit


valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git log --oneline
5b5b0ab (HEAD -> feature-dashboard) added new line info in file.txt
026b639 updated new line in file
cd30c76 update added for new dashboard.txt
7f7c827 added new dashboard.txt
74f4647 Initial init commit

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-dashboard)
$ git switch feature-auth
Switched to branch 'feature-auth'

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git log --oneline
e25cc70 (HEAD -> feature-auth) update info in file.txt
c8f4e50 Merge branch 'feature-dashboard' into feature-auth
026b639 updated new line in file
b18529e added new file file3
cd30c76 update added for new dashboard.txt
7f7c827 added new dashboard.txt
aa51e4e Created new login auth-login.txt
4edd51a add info in file2.txt
948e706 first change in file1.txt
74f4647 Initial init commit

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git log --oneline
f8807a9 (HEAD -> feature-auth) added new line 4 in file.txt
663cd90 added new line 3 in file.txt
6e0d548 added new line 2 in file.txt
9edf590 update merge conflicts from feature-dashboard to feature-auth
5b5b0ab (feature-dashboard) added new line info in file.txt
e25cc70 update info in file.txt
c8f4e50 Merge branch 'feature-dashboard' into feature-auth
026b639 updated new line in file
b18529e added new file file3
cd30c76 update added for new dashboard.txt
7f7c827 added new dashboard.txt
aa51e4e Created new login auth-login.txt
4edd51a add info in file2.txt
948e706 first change in file1.txt
74f4647 Initial init commit

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git rebase -i HEAD~3
[detached HEAD b4c4b94] added new line 2 in file.txt
 Date: Sun Jul 27 10:09:57 2025 +0300
 1 file changed, 3 insertions(+)
Successfully rebased and updated refs/heads/feature-auth.

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (feature-auth)
$ git log --oneline
b4c4b94 (HEAD -> feature-auth) added new line 2 in file.txt
9edf590 update merge conflicts from feature-dashboard to feature-auth
5b5b0ab (feature-dashboard) added new line info in file.txt
e25cc70 update info in file.txt
c8f4e50 Merge branch 'feature-dashboard' into feature-auth
026b639 updated new line in file
b18529e added new file file3
cd30c76 update added for new dashboard.txt
7f7c827 added new dashboard.txt
aa51e4e Created new login auth-login.txt
4edd51a add info in file2.txt
948e706 first change in file1.txt
74f4647 Initial init commit


valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git branch -a
  feature-auth
  feature-dashboard
  hotfix-security
* main
  remotes/origin/feature-auth
  remotes/origin/main

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git branch
  feature-auth
  feature-dashboard
  hotfix-security
* main


valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)
$ git reflog
b8e6c59 (HEAD -> main, origin/main) HEAD@{0}: commit: added README file with all working steps for Exercise 1
fbf3749 (hotfix-security) HEAD@{1}: checkout: moving from feature-auth to main
487338a (origin/feature-auth, feature-auth) HEAD@{2}: commit: added screenshots
b4c4b94 HEAD@{3}: checkout: moving from main to feature-auth
fbf3749 (hotfix-security) HEAD@{4}: checkout: moving from feature-auth to main
b4c4b94 HEAD@{5}: rebase (finish): returning to refs/heads/feature-auth
b4c4b94 HEAD@{6}: rebase (squash): added new line 2 in file.txt
f34e18c HEAD@{7}: rebase (squash): # This is a combination of 2 commits.
6e0d548 HEAD@{8}: rebase (start): checkout HEAD~3
f8807a9 HEAD@{9}: commit: added new line 4 in file.txt
663cd90 HEAD@{10}: commit: added new line 3 in file.txt
6e0d548 HEAD@{11}: commit: added new line 2 in file.txt
9edf590 HEAD@{12}: commit (merge): update merge conflicts from feature-dashboard to feature-auth
e25cc70 HEAD@{13}: checkout: moving from feature-dashboard to feature-auth
5b5b0ab (feature-dashboard) HEAD@{14}: commit: added new line info in file.txt
026b639 HEAD@{15}: checkout: moving from feature-auth to feature-dashboard
e25cc70 HEAD@{16}: commit: update info in file.txt
c8f4e50 HEAD@{17}: merge feature-dashboard: Merge made by the 'ort' strategy.
b18529e HEAD@{18}: checkout: moving from feature-dashboard to feature-auth
026b639 HEAD@{19}: commit: updated new line in file
cd30c76 HEAD@{20}: checkout: moving from feature-auth to feature-dashboard
b18529e HEAD@{21}: commit: added new file file3
aa51e4e HEAD@{22}: checkout: moving from main to feature-auth
fbf3749 (hotfix-security) HEAD@{23}: merge hotfix-security: Fast-forward
74f4647 HEAD@{24}: checkout: moving from hotfix-security to main
fbf3749 (hotfix-security) HEAD@{25}: commit: Fix bug in security login in secure-login.txt
74f4647 HEAD@{26}: checkout: moving from main to hotfix-security
74f4647 HEAD@{27}: checkout: moving from feature-dashboard to main
cd30c76 HEAD@{28}: commit: update added for new dashboard.txt
7f7c827 HEAD@{29}: commit: added new dashboard.txt
74f4647 HEAD@{30}: checkout: moving from main to feature-dashboard
74f4647 HEAD@{31}: checkout: moving from feature-auth to main
aa51e4e HEAD@{32}: commit: Created new login auth-login.txt
4edd51a HEAD@{33}: commit: add info in file2.txt
948e706 HEAD@{34}: commit: first change in file1.txt
74f4647 HEAD@{35}: checkout: moving from main to feature-auth
74f4647 HEAD@{36}: commit (initial): Initial init commit

valeri@win11-teslab MINGW64 /c/Exam/Multi-Branch Feature Development and Hotfix (main)