# Git-exercise-1

## bundle one

### exercise 1

```bash
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.
Try the new cross-platform PowerShell https://aka.ms/pscore6

PS C:\Users\TheGym\Desktop\Git exercises> git init
Initialized empty Git repository in C:/Users/TheGym/Desktop/Git exercises/.git/
PS C:\Users\TheGym\Desktop\Git exercises>
PS C:\Users\TheGym\Desktop\Git exercises> git branch -M main
PS C:\Users\TheGym\Desktop\Git exercises> echo "This is text filecreated in command line" > draft.txt
PS C:\Users\TheGym\Desktop\Git exercises> echo "this file will be deleted!" > "to delete.txt"
PS C:\Users\TheGym\Desktop\Git exercises> del "to delete.txt"
PS C:\Users\TheGym\Desktop\Git exercises> dir



Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/18/2022   5:04 PM             88 draft.txt

PS C:\Users\TheGym\Desktop\Git exercises> dir

    Directory: C:\Users\TheGym\Desktop\Git exercises

----                 -------------         ------ ----
-a----        10/18/2022   5:04 PM             88 draft.txt


PS C:\Users\TheGym\Desktop\Git exercises> ren "draft.txt" "draft Renamed.txt"
PS C:\Users\TheGym\Desktop\Git exercises> dir




Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/18/2022   5:04 PM             88 draft Renamed.txt


PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main: manuputated files"
[main (root-commit) f533d24] main: manuputated files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 draft Renamed.txt
PS C:\Users\TheGym\Desktop\Git exercises> git remote add origin https://github.com/serapieTuyishime/Git-exercise-1.git
PS C:\Users\TheGym\Desktop\Git exercises> git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream  origin main
To https://github.com/serapieTuyishime/Git-exercise-1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-1.git'
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\TheGym\Desktop\Git exercises> git pull
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 604 bytes | 23.00 KiB/s, done.
From https://github.com/serapieTuyishime/Git-exercise-1
 * [new branch]      main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-1.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main: connected remote and local"
On branch main
nothing to commit, working tree clean
PS C:\Users\TheGym\Desktop\Git exercises> git remote add origin
usage: git remote add [<options>] <name> <url>

    --tags                import all tags and associated objects when fetching
    -t, --track <branch>  branch(es) to track
                          master branch
                          set up remote as a mirror to push to or fetch from
PS C:\Users\TheGym\Desktop\Git exercises> git remote add origin https://github.com/serapieTuyierror: remote origin already exists.
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin main
To https://github.com/serapieTuyishime/Git-exercise-1.git
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

PS C:\Users\TheGym\Desktop\Git exercises> git push --force --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 293 bytes | 146.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/serapieTuyishime/Git-exercise-1.git
 + 13004b3...f533d24 main -> main (forced update)
branch 'main' set up to track 'origin/main'.

PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b  dev
fatal: a branch named 'dev' already exists
PS C:\Users\TheGym\Desktop\Git exercises> git switch dev
Switched to branch 'dev'
PS C:\Users\TheGym\Desktop\Git exercises> git branch --delete test
Deleted branch test (was f533d24).
PS C:\Users\TheGym\Desktop\Git exercises> git branch -a
* dev
  main
  remotes/origin/main
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "exercise one done bundle1 done"
On branch dev
nothing to commit, working tree clean
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises>
```

### exercise 2

```bash

PS C:\Users\TheGym\Desktop\Git exercises> git init
Reinitialized existing Git repository in C:/Users/TheGym/Desktop/Git exercises/.git/
PS C:\Users\TheGym\Desktop\Git exercises> git stash clear
PS C:\Users\TheGym\Desktop\Git exercises> echo "hdhhf" >"home.html"

PS C:\Users\TheGym\Desktop\Git exercises> git add home.html
d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> echo "this is
d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> git stash list
stash@{1}: WIP on dev: f533d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> echo "this is
the teams page" > "teams.html"
PS C:\Users\TheGym\Desktop\Git exercises> git stash
Saved working directory and index state WIP on dev: f533d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files
stash@{1}: WIP on dev: f533d24 main: manuputated files
stash@{2}: WIP on dev: f533d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> git checkout
stash@{1} about.html
error: unknown switch `e'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --guess               second guess 'git checkout <no-such-branch>' (default)
    --overlay             use overlay mode (default)
    -q, --quiet           suppress progress reporting
    --recurse-submodules[=<checkout>]
                          control recursive updating of
submodules
    --progress            force progress reporting
    -m, --merge           perform a 3-way merge with the new branch
    --conflict <style>    conflict style (merge, diff3,
or zdiff3)
    -d, --detach          detach HEAD at named commit
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -f, --force           force checkout (throw away local modifications)
    --orphan <new-branch>
                          new unparented branch
    --overwrite-ignore    update ignored files (default)    --ignore-other-worktrees
                          do not check if another worktree is holding the given ref
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unm    --ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character

PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files
stash@{1}: WIP on dev: f533d24 main: manuputated files
stash@{2}: WIP on dev: f533d24 main: manuputated files

PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files
stash@{1}: WIP on dev: f533d24 main: manuputated files
stash@{2}: WIP on dev: f533d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop
 stash@{0}
error: unknown switch `e'
usage: git stash pop [--index] [-q|--quiet] [<stash>]

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index
1
On branch dev
        new file:   about.html

Dropped refs/stash@{1} (bb7d051a451edb7afc8ce1ede56c34ca15382f26)
PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files
stash@{1}: WIP on dev: f533d24 main: manuputated files
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
Dropped refs/stash@{1} (0a2f674cebe3e4bdf3e1bfe42885bd4a7557b62f)
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m
"dev: did the stashing and unstashing"
[dev 0a3c229] dev: did the stashing and unstashing
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 about.html
 create mode 100644 home.html
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 921 bytes | 307.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
iting:
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.gi * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
PS C:\Users\TheGym\Desktop\Git exercises> git stash list

stash@{0}: WIP on dev: f533d24 main: manuputated files
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop
o
error: o is not a valid reference
PS C:\Users\TheGym\Desktop\Git exercises> git stash pop
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   teams.html

Dropped refs/stash@{0} (aab78323e4346404e68533e4c48053804a9859cc)
PS C:\Users\TheGym\Desktop\Git exercises> git reset
PS C:\Users\TheGym\Desktop\Git exercises> git reset
```

## bundle 2

### exercise one

```bash
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m
"ft/bundle-2 created new services"
[ft/bundle-2 461f146] ft/bundle-2 created new services
 2 files changed, 13 insertions(+)
 create mode 100644 services.html
 create mode 100644 teams.html
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin ft/bundle-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 894 bytes | 894.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/bundle-2
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
PS C:\Users\TheGym\Desktop\Git exercises>
```

### exercise 2

```bash

PS C:\Users\TheGym\Desktop\Git exercises> git pull
remote: Enumerating objects: 7, done.
remote: Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
From https://github.com/serapieTuyishime/Git-exercise-1
   f533d24..784e458  main       -> origin/main
Updating f533d24..784e458
Fast-forward
 README.md     | 281 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html    | Bin 0 -> 50 bytes
 home.html     | Bin 0 -> 1412 bytes
 4 files changed, 294 insertions(+)
 create mode 100644 README.md
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
PS C:\Users\TheGym\Desktop\Git exercises>
                                          git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin ft/service-redesign
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/service-redesign
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit --ammend --no-edit
error: unknown option `ammend'
usage: git commit [<options>] [--] <pathspec>...

    -q, --quiet           suppress summary after successful commit
    -v, --verbose         show diff in commit message template

Commit message options
    -F, --file <file>     read message from file
    --author <author>     override author for commit
    --date <date>         override date for commit
    -m, --message <message>
                          commit message
    -c, --reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --reuse-message <commit>
                          reuse message from specified commit
    --fixup [(amend|reword):]commit
                          use autosquash formatted message to fixup or amend/reword specified commit
    --squash <commit>     use autosquash formatted message to squash specified commit
    --reset-author        the commit is authored by me now (used with -C/-c/--amend)
    --trailer <trailer>   add custom trailer(s)
    -s, --signoff         add a Signed-off-by trailer
    -t, --template <file>
                          use specified template file
    -e, --edit            force edit of commit
    --cleanup <mode>      how to strip spaces and #comments from message
    --status              include status in commit message template
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --all             commit all changed files
    -i, --include         add specified files to index for commit
    --interactive         interactively add files
    -p, --patch           interactively add changes
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --dry-run             show what would be committed
    --short               show status concisely
    --ahead-behind        compute full ahead/behind values
    --porcelain           machine-readable output
    --long                show status in long format (default)
    -z, --null            terminate entries with NUL
    --amend               amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    -u, --untracked-files[=<mode>]
    --pathspec-from-file <file>
                          read pathspec from file

[ft/service-redesign d88eb4d] Merge pull request #1 from serapieTuyishime/ft/bundle-2
 Author: Chrissie <chrissiemhrk@gmail.com>
 Date: Wed Oct 19 17:36:45 2022 +0200
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin ft/service-redesign
PS C:\Users\TheGym\Desktop\Git exercises> git pull
Already up to date.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html

PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "ft/service-redesign: added changes on the services.html"
 1 file changed, 2 insertions(+)
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin ft/service-redesign
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/service-redesign
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git add .
 1 file changed, 5 insertions(+)
Enumerating objects: 5, done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/serapieTuyishime/Git-exercise-1.git
branch 'main' set up to track 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\Git exercises> git diff --iteractive
PS C:\Users\TheGym\Desktop\Git exercises> git diff --interactive
error: invalid option: --interactive
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
Switched to branch 'main'
PS C:\Users\TheGym\Desktop\Git exercises> git diff
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Aborting
PS C:\Users\TheGym\Desktop\Git exercises> git pull
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Unstaged changes after reset:
M       services.html
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\TheGym\Desktop\Git exercises> git reset
Unstaged changes after reset:
M       services.html
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Aborting
PS C:\Users\TheGym\Desktop\Git exercises> git add .
 1 file changed, 1 insertion(+)
Enumerating objects: 5, done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/serapieTuyishime/Git-exercise-1.git
   172e6ef..332147d  ft/service-redesign -> ft/service-redesign
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git pull
Already up to date.
PS C:\Users\TheGym\Desktop\Git exercises> git merge
Already up to date.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Aborting
PS C:\Users\TheGym\Desktop\Git exercises> git add .
[ft/service-redesign 189e520] Another conflic creation
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 371 bytes | 371.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/serapieTuyishime/Git-exercise-1.git
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git pull
Already up to date.
PS C:\Users\TheGym\Desktop\Git exercises> git diff
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 718 bytes | 20.00 KiB/s, done.
From https://github.com/serapieTuyishime/Git-exercise-1
   189e520..930351b  ft/service-redesign -> origin/ft/service-redesign
Already up to date.
PS C:\Users\TheGym\Desktop\Git exercises> git merge
Already up to date.
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main:resorved conflicts"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises>
```

## bundle 3

### exercise 1

```bash
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "ft/team-page: created teams page"
[ft/team-page 5d92c5e] ft/team-page: created teams page
 1 file changed, 18 insertions(+)
 create mode 100644 team.html
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin ft/team-page
To https://github.com/serapieTuyishime/Git-exercise-1.git
 ! [rejected]        ft/team-page -> ft/team-page (non-fast-forward)
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-1.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin ft/team-page
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 652 bytes | 652.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/team-page
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS C:\Users\TheGym\Desktop\Git exercises> git checkout ft/contact-page
 *  History restored


Try the new cross-platform PowerShell https://aka.ms/pscore6
PS C:\Users\TheGym\Desktop\Git exercises> git checkout main
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git branch -a
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
* main
  remotes/origin/dev
  remotes/origin/ft/bundle-2
  remotes/origin/ft/service-redesign
  remotes/origin/ft/team-page
  remotes/origin/main
PS C:\Users\TheGym\Desktop\Git exercises> git branch -D ft/team-page
Deleted branch ft/team-page (was 5d92c5e).
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main:created a team.html page"
[main 8c2762a] main:created a team.html page
 1 file changed, 12 insertions(+)
 create mode 100644 team.html
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin main
To https://github.com/serapieTuyishime/Git-exercise-1.git
 ! [rejected]        main -> main (fetch first)
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\TheGym\Desktop\Git exercises> git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
From https://github.com/serapieTuyishime/Git-exercise-1
   d17f69f..b62a8a4  main       -> origin/main
Merge made by the 'ort' strategy.
 README.md | 219 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 219 insertions(+)
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 787 bytes | 196.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
To https://github.com/serapieTuyishime/Git-exercise-1.git
branch 'main' set up to track 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git branch -a
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  list
* main
  remotes/origin/dev
  remotes/origin/ft/bundle-2
  remotes/origin/ft/service-redesign
  remotes/origin/ft/team-page
  remotes/origin/main
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git revert
usage: git revert [<options>] <commit-ish>...
   or: git revert <subcommand>

    --quit                end revert or cherry-pick sequence
    --continue            resume revert or cherry-pick sequence
    --abort               cancel revert or cherry-pick sequence
    --skip                skip current commit and continue
    --cleanup <mode>      how to strip spaces and #comments from message
    -n, --no-commit       don't automatically commit
    -e, --edit            edit the commit message
    -s, --signoff         add a Signed-off-by trailer
    -m, --mainline <parent-number>
                          select mainline parent
    --rerere-autoupdate   update the index with reused conflict resolution if possible
    --strategy <strategy>
                          merge strategy
    -X, --strategy-option <option>
                          option for merge strategy
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit
    --reference           use the 'reference' format to refer to commits

PS C:\Users\TheGym\Desktop\Git exercises> git reset --hard HEAD@{1}
error: unknown switch `e'
usage: git reset [--mixed | --soft | --hard | --merge | --keep] [-q] [<commit>]
   or: git reset [-q] [<tree-ish>] [--] <pathspec>...
   or: git reset [-q] [--pathspec-from-file [--pathspec-file-nul]] [<tree-ish>]
   or: git reset --patch [<tree-ish>] [--] [<pathspec>...]
   or: DEPRECATED: git reset [-q] [--stdin [-z]] [<tree-ish>]

    --no-refresh          skip refreshing the index after reset
    --mixed               reset HEAD and index
    --soft                reset only HEAD
    --merge               reset HEAD, index and working tree
    --keep                reset HEAD but keep local changes
    --recurse-submodules[=<reset>]
    -p, --patch           select hunks interactively
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character
    -z                    DEPRECATED (use --pathspec-file-nul instead): paths are separated with NUL character
    --stdin               DEPRECATED (use --pathspec-from-file=- instead): read paths from <stdin>

PS C:\Users\TheGym\Desktop\Git exercises> git reset 1
fatal: ambiguous argument '1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
PS C:\Users\TheGym\Desktop\Git exercises> git reset --hard 1
fatal: ambiguous argument '1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
PS C:\Users\TheGym\Desktop\Git exercises> git history
git: 'history' is not a git command. See 'git --help'.
PS C:\Users\TheGym\Desktop\Git exercises> git log
Merge: 8c2762a b62a8a4
Author: serapieTuyishime <tuyiserapie1@gmail.com>
Date:   Tue Oct 25 17:13:12 2022 +0200
    Merge branch 'main' of https://github.com/serapieTuyishime/Git-exercise-1

commit 8c2762a81c0a615758f1edf45cc17289a3aed8a4
Author: serapieTuyishime <tuyiserapie1@gmail.com>
Date:   Tue Oct 25 17:12:39 2022 +0200

    main:created a team.html page

commit b62a8a4123fbfff826b3d21d9255113a2987d9ac
Author: serapieTuyishime <70019756+serapieTuyishime@users.noreply.github.com>
Date:   Mon Oct 24 07:12:36 2022 -0700

PS C:\Users\TheGym\Desktop\Git exercises> git revert 8c2762a81c0a615758f1edf45cc17289a3aed8a
 1 file changed, 12 deletions(-)
PS C:\Users\TheGym\Desktop\Git exercises> git branch -a
  D
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
  list
* main
  remotes/origin/dev
  remotes/origin/ft/bundle-2
  remotes/origin/ft/service-redesign
  remotes/origin/main
PS C:\Users\TheGym\Desktop\Git exercises> git branch -a
  D
  dev
  ft/contact-page
  ft/service-redesign
  list
* main
  remotes/origin/dev
  remotes/origin/ft/bundle-2
  remotes/origin/ft/service-redesign
  remotes/origin/ft/team-page
  remotes/origin/main
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "ft/team-page : created a team-page and a team branch"
[ft/team-page dc7d59a] ft/team-page : created a team-page and a team branch
 create mode 100644 team.html
PS C:\Users\TheGym\Desktop\Git exercises> git push --set-upstream origin ft/team-page
Enumerating objects: 7, done.
Delta compression using up to 4 threads
Writing objects: 100% (5/5), 862 bytes | 431.00 KiB/s, done.
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/team-page
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/contact-page
fatal: a branch named 'ft/contact-page' already exists
PS C:\Users\TheGym\Desktop\Git exercises> git checkout  ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\TheGym\Desktop\Git exercises> git checkout  ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
PS C:\Users\TheGym\Desktop\Git exercises> git log
Author: serapieTuyishime <tuyiserapie1@gmail.com>

    ft/team-page : created a team-page and a team branch

commit 4a6d09ee5d89e071ff3ced32e9aec148cb428e46 (main)

    Revert "main:created a team.html page"
    This reverts commit 8c2762a81c0a615758f1edf45cc17289a3aed8a4.

commit 6dba56f38b56030340693e73c9e39a22d1d6c84e (origin/main)
Merge: 8c2762a b62a8a4
Author: serapieTuyishime <tuyiserapie1@gmail.com>
PS C:\Users\TheGym\Desktop\Git exercises> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\TheGym\Desktop\Git exercises> git cherry-pick dc7d59aa4a5f611327842f3c44896d3146272ed5
[ft/contact-page 18d09c9] ft/team-page : created a team-page and a team branch
 Date: Tue Oct 25 17:24:14 2022 +0200
 1 file changed, 13 insertions(+)
 create mode 100644 team.html
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "ft:contact-page have edited team.tml"
 1 file changed, 1 insertion(+)
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/contact-page
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "ft/faq-page was created"
[ft/faq-page 68722d8] ft/faq-page was created
 create mode 100644 FAq.html
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 492 bytes | 123.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/faq-page
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\TheGym\Desktop\Git exercises> git log
Author: serapieTuyishime <tuyiserapie1@gmail.com>
Date:   Tue Oct 25 17:35:05 2022 +0200

    ft/faq-page was created

commit 52412f38f890968d7197af8c267cf77bd3bc3486 (origin/ft/contact-page, ft/contact-page)
Author: serapieTuyishime <tuyiserapie1@gmail.com>
Date:   Tue Oct 25 17:32:12 2022 +0200
    ft:contact-page have edited team.tml
commit 18d09c90056f1bf2f939dd926e400c7cb9a47a9d
Author: serapieTuyishime <tuyiserapie1@gmail.com>
Date:   Tue Oct 25 17:24:14 2022 +0200
PS C:\Users\TheGym\Desktop\Git exercises> git revert dc7d59aa4a5f611327842f3c44896d3146272ed5
CONFLICT (modify/delete): team.html deleted in parent of dc7d59a (ft/team-page : created a team-page and a team branch) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert dc7d59a... ft/team-page : created a team-page and a team branch
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".
PS C:\Users\TheGym\Desktop\Git exercises> git revert dc7d59aa4a5f611327842f3c44896d3146272ed5
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed
PS C:\Users\TheGym\Desktop\Git exercises> git add .
[ft/faq-page 8113593] ft: faq trying to revert
 1 file changed, 14 deletions(-)
PS C:\Users\TheGym\Desktop\Git exercises> git revert dc7d59aa4a5f611327842f3c44896d3146272ed5
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "ft/faq-page: reverted other people's changes"
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin ft:faq-page
error: src refspec ft does not match any
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-1.git'
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 237 bytes | 237.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/serapieTuyishime/Git-exercise-1.git
   68722d8..8113593  ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\TheGym\Desktop\Git exercises>
```

## bundle3

### exercise 2

```bash
PS C:\Users\TheGym\Desktop\Git exercises> git branch ft/home-page-redesign
PS C:\Users\TheGym\Desktop\Git exercises> git branch -a
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
  main
  remotes/origin/dev
  remotes/origin/ft/bundle-2
  remotes/origin/ft/contact-page
  remotes/origin/ft/faq-page
  remotes/origin/ft/service-redesign
  remotes/origin/ft/team-page
  remotes/origin/main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main: made some changes da!"
[main 4f91db3] main: made some changes da!
 1 file changed, 0 insertions(+), 0 deletions(-)
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin main
To https://github.com/serapieTuyishime/Git-exercise-1.git
 ! [rejected]        main -> main (fetch first)
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\TheGym\Desktop\Git exercises> git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
From https://github.com/serapieTuyishime/Git-exercise-1
Merge made by the 'ort' strategy.
 README.md | 346 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 346 insertions(+)
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin main
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 767 bytes | 767.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/serapieTuyishime/Git-exercise-1.git
   fbc7586..47eea8e  main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "ft:redesigned the homepage"
[ft/home-page-redesign ffdd6c6] ft:redesigned the homepage
 1 file changed, 0 insertions(+), 0 deletions(-)
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.80 KiB | 461.00 KiB/s, done.
Total 14 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/serapieTuyishime/Git-exercise-1/pull/new/ft/home-page-redesign
remote:
To https://github.com/serapieTuyishime/Git-exercise-1.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
PS C:\Users\TheGym\Desktop\Git exercises>
```
## bundle 4
### exercise 1
```bash
PS C:\Users\TheGym\Desktop\Git exercises> git remote add git-copy https://github.com/serapieTuyishime/Git-exercise-2.git
PS C:\Users\TheGym\Desktop\Git exercises> git add .
PS C:\Users\TheGym\Desktop\Git exercises> git commit -m "main: added a new repo"
[main 8fcaa31] main: added a new repo
 2 files changed, 157 insertions(+), 69 deletions(-)
PS C:\Users\TheGym\Desktop\Git exercises> git push -u origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.41 KiB | 721.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/serapieTuyishime/Git-exercise-1.git
   47eea8e..8fcaa31  main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\TheGym\Desktop\Git exercises> git push git-copy main
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-2.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\TheGym\Desktop\Git exercises> git push git-copy main
To https://github.com/serapieTuyishime/Git-exercise-2.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/serapieTuyishime/Git-exercise-2.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\TheGym\Desktop\Git exercises> git push -f  git-copy main
Enumerating objects: 42, done.
Counting objects: 100% (42/42), done.
Delta compression using up to 4 threads
Compressing objects: 100% (41/41), done.
Writing objects: 100% (42/42), 14.54 KiB | 930.00 KiB/s, done.
Total 42 (delta 18), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (18/18), done.
To https://github.com/serapieTuyishime/Git-exercise-2.git
 + fa0c6d5...8fcaa31 main -> main (forced update)
PS C:\Users\TheGym\Desktop\Git exercises> 
```
