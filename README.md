# GIT_Ex8
surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (master)
$ git branch my-feature

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (master)
$ git checkout my-feature
Switched to branch 'my-feature'

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (my-feature)
$ git add about.html

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (my-feature)
$ git commit -m "Adding about.html"
[my-feature 594a070] Adding about.html
 1 file changed, 9 insertions(+)
 create mode 100644 about.html

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (my-feature)
$ git tag COMMIT2

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (my-feature)
$ git checkout master
Switched to branch 'master'

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (master)
$ git status
On branch master
nothing to commit, working tree clean

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (master)
$ git merge my-feature
Updating dcb96a8..594a070
Fast-forward
 about.html | 9 +++++++++
 1 file changed, 9 insertions(+)
 create mode 100644 about.html

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (master)
$ git log
commit 594a070c2ad29a0d75dd6f0e5ddb78407beee132 (HEAD -> master, tag: COMMIT2, my-feature)
Author: Surbhi Jain <surbhijain09@gmail.com>
Date:   Fri Jan 14 18:33:54 2022 -0500

    Adding about.html

commit dcb96a8c8bfb745e0924f62844a42ba28df01988 (tag: Commit1)
Author: Surbhi Jain <surbhijain09@gmail.com>
Date:   Fri Jan 14 18:30:02 2022 -0500

    Adding index.html

surbh@DESKTOP-UQB074A MINGW64 ~/Desktop/GIT_Ex8 (master)
$ git push https://github.com/SurbhiJain09/GIT_Ex8.git
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 623 bytes | 77.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/SurbhiJain09/GIT_Ex8.git
 * [new branch]      master -> master

