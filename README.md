# Codefile
Microsoft Windows [Version 10.0.19044.2130]
(c) Microsoft Corporation. All rights reserved.

C:\Apps\Murali\Git-Hub>dir
 Volume in drive C is OS
 Volume Serial Number is F0DD-D49F

 Directory of C:\Apps\Murali\Git-Hub

14-10-2022  22:14    <DIR>          .
14-10-2022  22:14    <DIR>          ..
               0 File(s)              0 bytes
               2 Dir(s)  256,385,396,736 bytes free

C:\Apps\Murali\Git-Hub>mkdir repo1

C:\Apps\Murali\Git-Hub>dir
 Volume in drive C is OS
 Volume Serial Number is F0DD-D49F

 Directory of C:\Apps\Murali\Git-Hub

14-10-2022  22:15    <DIR>          .
14-10-2022  22:15    <DIR>          ..
14-10-2022  22:15    <DIR>          repo1
               0 File(s)              0 bytes
               3 Dir(s)  256,385,323,008 bytes free

C:\Apps\Murali\Git-Hub>cd repo1

C:\Apps\Murali\Git-Hub\repo1>git status
fatal: not a git repository (or any of the parent directories): .git

C:\Apps\Murali\Git-Hub\repo1>git init
Initialized empty Git repository in C:/Apps/Murali/Git-Hub/repo1/.git/

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

C:\Apps\Murali\Git-Hub\repo1>git branch

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file1.txt.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Apps\Murali\Git-Hub\repo1>git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

C:\Apps\Murali\Git-Hub\repo1>git add .

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file1.txt.txt


C:\Apps\Murali\Git-Hub\repo1>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file1.txt.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file2.txt.txt


C:\Apps\Murali\Git-Hub\repo1>git add file2.txt.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file1.txt.txt
        new file:   file2.txt.txt


C:\Apps\Murali\Git-Hub\repo1>git rm --cached file2.txt.txt
rm 'file2.txt.txt'

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   file1.txt.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file2.txt.txt


C:\Apps\Murali\Git-Hub\repo1>git commint -m "firstcommit date"
git: 'commint' is not a git command. See 'git --help'.

The most similar command is
        commit

C:\Apps\Murali\Git-Hub\repo1>git commit -m "firstcommit date"
[master (root-commit) dab298c] firstcommit date
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file1.txt.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file2.txt.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Apps\Murali\Git-Hub\repo1>git log
commit dab298c7c689c2233f94e8afcf631ec8b6088d78 (HEAD -> master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git add .

C:\Apps\Murali\Git-Hub\repo1>git commit -m "2ndcommit date"
[master d79337c] 2ndcommit date
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file2.txt.txt

C:\Apps\Murali\Git-Hub\repo1>git log
commit d79337c88701b70b20f5e268a934b985dac56169 (HEAD -> master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    file2.txt.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Apps\Murali\Git-Hub\repo1>git add file2.txt.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    file2.txt.txt


C:\Apps\Murali\Git-Hub\repo1>git commit -m "file2  deleted"
[master 798436e] file2  deleted
 1 file changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 file2.txt.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git log
commit 798436e0f0f16dccb339565dc6d730c968e0c0df (HEAD -> master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git checkout -b SubMaster
Switched to a new branch 'SubMaster'

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git log
commit 798436e0f0f16dccb339565dc6d730c968e0c0df (HEAD -> SubMaster, master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    file1.txt.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file1.txt
        file3.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Apps\Murali\Git-Hub\repo1>git add .

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    file1.txt.txt -> file1.txt
        new file:   file3.txt


C:\Apps\Murali\Git-Hub\repo1>git commit -m "subbranch added with file modification"
[SubMaster 4b24e37] subbranch added with file modification
 2 files changed, 0 insertions(+), 0 deletions(-)
 rename file1.txt.txt => file1.txt (100%)
 create mode 100644 file3.txt

C:\Apps\Murali\Git-Hub\repo1>git log
commit 4b24e37bc9a71c41f0e41dbec3cda17989bc19f1 (HEAD -> SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 798436e0f0f16dccb339565dc6d730c968e0c0df (master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git checkout master
Switched to branch 'master'

C:\Apps\Murali\Git-Hub\repo1>git checkout submaster
Switched to branch 'submaster'

C:\Apps\Murali\Git-Hub\repo1>git checkout master
Switched to branch 'master'

C:\Apps\Murali\Git-Hub\repo1>git log
commit 798436e0f0f16dccb339565dc6d730c968e0c0df (HEAD -> master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git branch
  SubMaster
* master

C:\Apps\Murali\Git-Hub\repo1>git checkout submaster
Switched to branch 'submaster'

C:\Apps\Murali\Git-Hub\repo1>git branch
  SubMaster
  master

C:\Apps\Murali\Git-Hub\repo1>git checkout SubMaster
Switched to branch 'SubMaster'

C:\Apps\Murali\Git-Hub\repo1>git branch
* SubMaster
  master

C:\Apps\Murali\Git-Hub\repo1>git branch -u master
Branch 'SubMaster' set up to track local branch 'master'.

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch is ahead of 'master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git checkout master
Switched to branch 'master'

C:\Apps\Murali\Git-Hub\repo1>git branch
  SubMaster
* master

C:\Apps\Murali\Git-Hub\repo1>git add file4.txt

C:\Apps\Murali\Git-Hub\repo1>git commit
Aborting commit due to empty commit message.

C:\Apps\Murali\Git-Hub\repo1>git commit -m "file 4 added newly"
[master 8f2e83b] file 4 added newly
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file4.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git log
commit 8f2e83bf4f82130585b9170aaa35c5b4db785850 (HEAD -> master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:36:45 2022 +0530

    file 4 added newly

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git checkout SubMaster
Switched to branch 'SubMaster'
Your branch and 'master' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

C:\Apps\Murali\Git-Hub\repo1>git branch
* SubMaster
  master

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch and 'master' have diverged,
and have 1 and 1 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git log
commit 4b24e37bc9a71c41f0e41dbec3cda17989bc19f1 (HEAD -> SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git rebase
Successfully rebased and updated refs/heads/SubMaster.

C:\Apps\Murali\Git-Hub\repo1>git log
commit bc39e702b5d3d093cb9d697b742805fa65e5837c (HEAD -> SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 8f2e83bf4f82130585b9170aaa35c5b4db785850 (master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:36:45 2022 +0530

    file 4 added newly

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch is ahead of 'master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push . HEAD:master

To push to the branch of the same name on the remote, use

    git push . HEAD

To choose either option permanently, see push.default in 'git help config'.

C:\Apps\Murali\Git-Hub\repo1>git push master
fatal: 'master' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

C:\Apps\Murali\Git-Hub\repo1>git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push . HEAD:master

To push to the branch of the same name on the remote, use

    git push . HEAD

To choose either option permanently, see push.default in 'git help config'.

C:\Apps\Murali\Git-Hub\repo1>git push -help
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --repo <repository>   repository
    --all                 push all refs
    --mirror              mirror all refs
    -d, --delete          delete refs
    --tags                push tags (can't be used with --all or --mirror)
    -n, --dry-run         dry run
    --porcelain           machine-readable output
    -f, --force           force updates
    --force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --force-if-includes   require remote updates to be integrated locally
    --recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --thin                use thin pack
    --receive-pack <receive-pack>
                          receive pack program
    --exec <receive-pack>
                          receive pack program
    -u, --set-upstream    set upstream for git pull/status
    --progress            force progress reporting
    --prune               prune locally removed refs
    --no-verify           bypass pre-push hook
    --follow-tags         push missing but relevant tags
    --signed[=(yes|no|if-asked)]
                          GPG sign the push
    --atomic              request atomic transaction on remote side
    -o, --push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only


C:\Apps\Murali\Git-Hub\repo1>git push --all
Everything up-to-date

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch is ahead of 'master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git push . master
Everything up-to-date

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch is ahead of 'master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git fetch -p
From .
 * branch            master     -> FETCH_HEAD

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch is ahead of 'master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push . HEAD:master

To push to the branch of the same name on the remote, use

    git push . HEAD

To choose either option permanently, see push.default in 'git help config'.

C:\Apps\Murali\Git-Hub\repo1> git push . HEAD:master
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To .
   8f2e83b..bc39e70  HEAD -> master

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch is up to date with 'master'.

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git checkout master
Switched to branch 'master'

C:\Apps\Murali\Git-Hub\repo1>git log
commit bc39e702b5d3d093cb9d697b742805fa65e5837c (HEAD -> master, SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 8f2e83bf4f82130585b9170aaa35c5b4db785850
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:36:45 2022 +0530

    file 4 added newly

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git add .\

C:\Apps\Murali\Git-Hub\repo1>git add .

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file5.txt


C:\Apps\Murali\Git-Hub\repo1>git commit -m "file 5 added in master"
[master 6ebe2f7] file 5 added in master
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file5.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git log
commit 6ebe2f7016941ef0e33f673ff65c9671fba2116f (HEAD -> master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:55:34 2022 +0530

    file 5 added in master

commit bc39e702b5d3d093cb9d697b742805fa65e5837c (SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 8f2e83bf4f82130585b9170aaa35c5b4db785850
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:36:45 2022 +0530

    file 4 added newly

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file6.txt
        file7.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Apps\Murali\Git-Hub\repo1>git add file6.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file6.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file7.txt


C:\Apps\Murali\Git-Hub\repo1>git commit -m "file 6 added"
[master eb2ad88] file 6 added
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file6.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file7.txt

nothing added to commit but untracked files present (use "git add" to track)

C:\Apps\Murali\Git-Hub\repo1>git add .

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file7.txt


C:\Apps\Murali\Git-Hub\repo1>git commit -m "file 7 added"
[master efdb0f3] file 7 added
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file7.txt

C:\Apps\Murali\Git-Hub\repo1>git status
On branch master
nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git log
commit efdb0f323df59b39922fca4772480622a0282ba9 (HEAD -> master)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:57:41 2022 +0530

    file 7 added

commit eb2ad880f3b83f2d37b31835d1600b428cd5f12c
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:56:56 2022 +0530

    file 6 added

commit 6ebe2f7016941ef0e33f673ff65c9671fba2116f
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:55:34 2022 +0530

    file 5 added in master

commit bc39e702b5d3d093cb9d697b742805fa65e5837c (SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 8f2e83bf4f82130585b9170aaa35c5b4db785850
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:36:45 2022 +0530

    file 4 added newly

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git checkout SubMaster
Switched to branch 'SubMaster'
Your branch is behind 'master' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

C:\Apps\Murali\Git-Hub\repo1>git cherry-pick eb2ad880f3b83f2d37b31835d1600b428cd5f12c
[SubMaster 96c18c7] file 6 added
 Date: Fri Oct 14 22:56:56 2022 +0530
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file6.txt

C:\Apps\Murali\Git-Hub\repo1>git log
commit 96c18c7436cc8866c100d6d90385ee1ea4e93d63 (HEAD -> SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:56:56 2022 +0530

    file 6 added

commit bc39e702b5d3d093cb9d697b742805fa65e5837c
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 8f2e83bf4f82130585b9170aaa35c5b4db785850
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:36:45 2022 +0530

    file 4 added newly

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch and 'master' have diverged,
and have 1 and 3 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push . HEAD:master

To push to the branch of the same name on the remote, use

    git push . HEAD

To choose either option permanently, see push.default in 'git help config'.

C:\Apps\Murali\Git-Hub\repo1> git push . HEAD:master
To .
 ! [rejected]        HEAD -> master (non-fast-forward)
error: failed to push some refs to '.'
hint: Updates were rejected because a pushed branch tip is behind its remote
hint: counterpart. Check out this branch and integrate the remote changes
hint: (e.g. 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

C:\Apps\Murali\Git-Hub\repo1> git push . HEAD:master -f
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To .
 + efdb0f3...96c18c7 HEAD -> master (forced update)

C:\Apps\Murali\Git-Hub\repo1>git status
On branch SubMaster
Your branch is up to date with 'master'.

nothing to commit, working tree clean

C:\Apps\Murali\Git-Hub\repo1>git checkout master
Switched to branch 'master'

C:\Apps\Murali\Git-Hub\repo1>git reflog
96c18c7 (HEAD -> master, SubMaster) HEAD@{0}: checkout: moving from SubMaster to master
96c18c7 (HEAD -> master, SubMaster) HEAD@{1}: cherry-pick: file 6 added
bc39e70 HEAD@{2}: checkout: moving from master to SubMaster
efdb0f3 HEAD@{3}: commit: file 7 added
eb2ad88 HEAD@{4}: commit: file 6 added
6ebe2f7 HEAD@{5}: commit: file 5 added in master
bc39e70 HEAD@{6}: checkout: moving from SubMaster to master
bc39e70 HEAD@{7}: rebase (finish): returning to refs/heads/SubMaster
bc39e70 HEAD@{8}: rebase (pick): subbranch added with file modification
8f2e83b HEAD@{9}: rebase (start): checkout refs/heads/master
4b24e37 HEAD@{10}: checkout: moving from master to SubMaster
8f2e83b HEAD@{11}: commit: file 4 added newly
798436e HEAD@{12}: checkout: moving from SubMaster to master
4b24e37 HEAD@{13}: checkout: moving from submaster to SubMaster
4b24e37 HEAD@{14}: checkout: moving from master to submaster
798436e HEAD@{15}: checkout: moving from submaster to master
4b24e37 HEAD@{16}: checkout: moving from master to submaster
798436e HEAD@{17}: checkout: moving from SubMaster to master
4b24e37 HEAD@{18}: commit: subbranch added with file modification
798436e HEAD@{19}: checkout: moving from master to SubMaster
798436e HEAD@{20}: commit: file2 deleted
d79337c HEAD@{21}: commit: 2ndcommit date
dab298c HEAD@{22}: commit (initial): firstcommit date

C:\Apps\Murali\Git-Hub\repo1>git fetch --all

C:\Apps\Murali\Git-Hub\repo1>git log
commit 96c18c7436cc8866c100d6d90385ee1ea4e93d63 (HEAD -> master, SubMaster)
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:56:56 2022 +0530

    file 6 added

commit bc39e702b5d3d093cb9d697b742805fa65e5837c
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:30:06 2022 +0530

    subbranch added with file modification

commit 8f2e83bf4f82130585b9170aaa35c5b4db785850
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:36:45 2022 +0530

    file 4 added newly

commit 798436e0f0f16dccb339565dc6d730c968e0c0df
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:25:51 2022 +0530

    file2  deleted

commit d79337c88701b70b20f5e268a934b985dac56169
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:24:25 2022 +0530

    2ndcommit date

commit dab298c7c689c2233f94e8afcf631ec8b6088d78
Author: Suganya Panneerselvam <suganya.panneerselvam@dataquest.com.au>
Date:   Fri Oct 14 22:23:05 2022 +0530

    firstcommit date

C:\Apps\Murali\Git-Hub\repo1>
