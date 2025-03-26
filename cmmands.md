 'git help git' for an overview of the system.
ubuntu@ip-172-31-92-81:~$ git --version
git version 2.43.0
ubuntu@ip-172-31-92-81:~$ pwd
/home/ubuntu
ubuntu@ip-172-31-92-81:~$ mkdir git-tutorial
ubuntu@ip-172-31-92-81:~$ ls
git-tutorial
ubuntu@ip-172-31-92-81:~$ cd git-tutorial/
ubuntu@ip-172-31-92-81:~/git-tutorial$ vim hellio-dosto.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
Initialized empty Git repository in /home/ubuntu/git-tutorial/.git/
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls -la
total 16
drwxrwxr-x 3 ubuntu ubuntu 4096 Mar 26 10:07 .
drwxr-x--- 5 ubuntu ubuntu 4096 Mar 26 10:00 ..
drwxrwxr-x 7 ubuntu ubuntu 4096 Mar 26 10:07 .git
-rw-rw-r-- 1 ubuntu ubuntu   24 Mar 26 10:00 hellio-dosto.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
hellio-dosto.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hellio-dosto.txt

nothing added to commit but untracked files present (use "git add" to track)
ubuntu@ip-172-31-92-81:~/git-tutorial$ touch nibba.txt nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
hellio-dosto.txt  nibba.txt  nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hellio-dosto.txt
        nibba.txt
        nibbi.txt

nothing added to commit but untracked files present (use "git add" to track)
ubuntu@ip-172-31-92-81:~/git-tutorial$ rm hellio-dosto.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        nibba.txt
        nibbi.txt

nothing added to commit but untracked files present (use "git add" to track)
ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibb.txt
fatal: pathspec 'nibb.txt' did not match any files
ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   nibbi.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        nibba.txt

ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   nibbi.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        nibba.txt

ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibba.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   nibba.txt
        new file:   nibbi.txt

ubuntu@ip-172-31-92-81:~/git-tutorial$ git rm --cached  nibba.txt
rm 'nibba.txt'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   nibbi.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        nibba.txt

ubuntu@ip-172-31-92-81:~/git-tutorial$ git add  nibba.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   nibba.txt
        new file:   nibbi.txt

ubuntu@ip-172-31-92-81:~/git-tutorial$ git commit -m "adding nibba nibbi"
[master (root-commit) c4e67e2] adding nibba nibbi
 Committer: Ubuntu <ubuntu@ip-172-31-92-81.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 nibba.txt
 create mode 100644 nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master
nothing to commit, working tree clean
ubuntu@ip-172-31-92-81:~/git-tutorial$ rm nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    nibbi.txt

no changes added to commit (use "git add" and/or "git commit -a")
ubuntu@ip-172-31-92-81:~/git-tutorial$ git restore nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master
nothing to commit, working tree clean
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
nibba.txt  nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ client_loop: send disconnect: Connection reset

C:\Users\vibha\downloads>ssh -i "anant11.pem" ubuntu@ec2-3-83-24-158.compute-1.amazonaws.com
Welcome to Ubuntu 24.04.2 LTS (GNU/Linux 6.8.0-1024-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/pro

 System information as of Wed Mar 26 11:20:38 UTC 2025

  System load:  0.0               Processes:             105
  Usage of /:   25.4% of 6.71GB   Users logged in:       0
  Memory usage: 20%               IPv4 address for enX0: 172.31.92.81
  Swap usage:   0%


Expanded Security Maintenance for Applications is not enabled.

0 updates can be applied immediately.

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status


The list of available updates is more than a week old.
To check for new updates run: sudo apt update

Last login: Wed Mar 26 09:54:30 2025 from 103.102.144.121
To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

ubuntu@ip-172-31-92-81:~$ cd git-tutorial/
ubuntu@ip-172-31-92-81:~/git-tutorial$ git config --global user.name "<vibhavari saraf>"
ubuntu@ip-172-31-92-81:~/git-tutorial$ git config --global user.name "<vibhavarisaraf4555>"
ubuntu@ip-172-31-92-81:~/git-tutorial$ git config --global user.email "<vibhavarisaraf5444@gmail.com>"
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
nibba.txt  nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ vim nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   nibbi.txt

no changes added to commit (use "git add" and/or "git commit -a")
ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git commit -m "added new changes"
[master f219bd6] added new changes
 1 file changed, 1 insertion(+)
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log
commit f219bd66763c95916bb948224d5180baa565237a (HEAD -> master)
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:16:03 2025 +0000

    added new changes

commit c4e67e2bb1f0a66fdcbdc0e841e300e5ae2d7051
Author: Ubuntu <ubuntu@ip-172-31-92-81.ec2.internal>
Date:   Wed Mar 26 10:20:33 2025 +0000

    adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ vim nibba.txt

ubuntu@ip-172-31-92-81:~/git-tutorial$ git commit -m "aqdded nibbaa changes"
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   nibba.txt

no changes added to commit (use "git add" and/or "git commit -a")
ubuntu@ip-172-31-92-81:~/git-tutorial$ git commit -m "added nibbaa changes"
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   nibba.txt

no changes added to commit (use "git add" and/or "git commit -a")
ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibba.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git commit -m "added nibbaa changes"
[master fa8f010] added nibbaa changes
 1 file changed, 1 insertion(+)
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log
commit fa8f0103a2a8a1f21480e39077dce53936e24a50 (HEAD -> master)
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:22:26 2025 +0000

    added nibbaa changes

commit f219bd66763c95916bb948224d5180baa565237a
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:16:03 2025 +0000

    added new changes

commit c4e67e2bb1f0a66fdcbdc0e841e300e5ae2d7051
Author: Ubuntu <ubuntu@ip-172-31-92-81.ec2.internal>
Date:   Wed Mar 26 10:20:33 2025 +0000

    adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout -b dev
Switched to a new branch 'dev'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch dev
nothing to commit, working tree clean
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout master
Switched to branch 'master'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master
nothing to commit, working tree clean
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout dev
Switched to branch 'dev'
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
nibba.txt  nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ touch nibbu.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        nibbu.txt

nothing added to commit but untracked files present (use "git add" to track)
ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibbu.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git commit -m nibbu.txt
[dev 2521f90] nibbu.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 nibbu.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch dev
nothing to commit, working tree clean
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout master
Switched to branch 'master'
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
nibba.txt  nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git logs
git: 'logs' is not a git command. See 'git --help'.

The most similar command is
        log
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log
commit fa8f0103a2a8a1f21480e39077dce53936e24a50 (HEAD -> master)
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:22:26 2025 +0000

    added nibbaa changes

commit f219bd66763c95916bb948224d5180baa565237a
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:16:03 2025 +0000

    added new changes

commit c4e67e2bb1f0a66fdcbdc0e841e300e5ae2d7051
Author: Ubuntu <ubuntu@ip-172-31-92-81.ec2.internal>
Date:   Wed Mar 26 10:20:33 2025 +0000

    adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout dev
Switched to branch 'dev'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log
commit 2521f9078d99b452836001e1ae80080dd8db6bc0 (HEAD -> dev)
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:32:02 2025 +0000

    nibbu.txt

commit fa8f0103a2a8a1f21480e39077dce53936e24a50 (master)
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:22:26 2025 +0000

    added nibbaa changes

commit f219bd66763c95916bb948224d5180baa565237a
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:16:03 2025 +0000

    added new changes

commit c4e67e2bb1f0a66fdcbdc0e841e300e5ae2d7051
Author: Ubuntu <ubuntu@ip-172-31-92-81.ec2.internal>
Date:   Wed Mar 26 10:20:33 2025 +0000

    adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch dev
nothing to commit, working tree clean
ubuntu@ip-172-31-92-81:~/git-tutorial$ git branch
* dev
  master
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout master
Switched to branch 'master'
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
nibba.txt  nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ git branch
  dev
* master
ubuntu@ip-172-31-92-81:~/git-tutorial$ git switch dev
Switched to branch 'dev'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout master
Switched to branch 'master'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log --oneline
fa8f010 (HEAD -> master) added nibbaa changes
f219bd6 added new changes
c4e67e2 adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ git status
On branch master
nothing to commit, working tree clean
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout dev
Switched to branch 'dev'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log --oneline
2521f90 (HEAD -> dev) nibbu.txt
fa8f010 (master) added nibbaa changes
f219bd6 added new changes
c4e67e2 adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout -b from-dev
Switched to a new branch 'from-dev'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log
commit 2521f9078d99b452836001e1ae80080dd8db6bc0 (HEAD -> from-dev, dev)
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:32:02 2025 +0000

    nibbu.txt

commit fa8f0103a2a8a1f21480e39077dce53936e24a50 (master)
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:22:26 2025 +0000

    added nibbaa changes

commit f219bd66763c95916bb948224d5180baa565237a
Author: vibhavarisaraf4555 <vibhavarisaraf5444@gmail.com>
Date:   Wed Mar 26 12:16:03 2025 +0000

    added new changes

commit c4e67e2bb1f0a66fdcbdc0e841e300e5ae2d7051
Author: Ubuntu <ubuntu@ip-172-31-92-81.ec2.internal>
Date:   Wed Mar 26 10:20:33 2025 +0000

    adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout master
Switched to branch 'master'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout -b from-dev
fatal: a branch named 'from-dev' already exists
ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout -b from-master
Switched to a new branch 'from-master'
ubuntu@ip-172-31-92-81:~/git-tutorial$ git log --oneline
fa8f010 (HEAD -> from-master, master) added nibbaa changes
f219bd6 added new changes
c4e67e2 adding nibba nibbi
ubuntu@ip-172-31-92-81:~/git-tutorial$ ls
nibba.txt  nibbi.txt
ubuntu@ip-172-31-92-81:~/git-tutorial$ client_loop: send disconnect: Connection reset

C:\Users\vibha\downloads>ssh -i "anant11.pem" ubuntu@ec2-3-83-24-158.compute-1.amazonaws.com
Welcome to Ubuntu 24.04.2 LTS (GNU/Linux 6.8.0-1024-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/pro

 System information as of Wed Mar 26 13:24:32 UTC 2025

  System load:  0.0               Processes:             106
  Usage of /:   25.4% of 6.71GB   Users logged in:       1
  Memory usage: 20%               IPv4 address for enX0: 172.31.92.81
  Swap usage:   0%


Expanded Security Maintenance for Applications is not enabled.

0 updates can be applied immediately.

Enable ESM Apps to receive additional future security updates.
See https://ubuntu.com/esm or run: sudo pro status


The list of available updates is more than a week old.
To check for new updates run: sudo apt update

Last login: Wed Mar 26 11:20:39 2025 from 103.102.144.121
To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

ubuntu@ip-172-31-92-81:~$ ls
git-tutorial
ubuntu@ip-172-31-92-81:~$ cd git-tutorial/
ubuntu@ip-172-31-92-81:~/git-tutorial$ client_loop: send disconnect: Connection reset

C:\Users\vibha\downloads>
