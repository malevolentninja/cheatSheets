


| Keyword | Explanation |
|--------|:-------------------------------:|
| git config --global user.name "[firstname lastname]" | set a name that is identifiable for credit when review version history |
| git config --global user.email "[valid-email]" | set an email address that will be associated with each history marker|
| git config --global color.ui autot | set automatic command line colouring git for easy reviewing
| Setup and Init| |
| git init | initialize an existing directory as a git respository|
| git clone [url] | retrieve an entire respository from a hosted location via URL|
| Stage and Snapshot|
| git status| show modified files in working directory, staged for your next commit|
| git add [file] | add a file as it looks now to your next commit (stage)|
| git add . | add all current changes|
| git commit -m "[descriptive message]"| commit your staged content as a new commit|
| git add -p <file> | add some changes in <file> to the next commit|
| git reset [file] | unstage a file while retaining the changes in working directory|
| git diff | diff of what is changed but not staged|
| git diff --staged| diff of what is changed but not yet committed|
| Branches and Merges| |
| git branch| list your branches a* will appear next to the currently active branch|
| git branch [branch-name]| create |a new branch at the current commit|
| git branch -d <branch>| delete a local branch|
| git branch -av| list all existing branches|
| git merge <branch>| merge <branch> into your current HEAD|
| git tag <tag-name>| mark the current commit with a tag |
| git checkout| switch to another branch and check it out into your working directory|
| git checkout <branch>| switch to another branch and check it out into your working directory|
| git branch <new-branch> | create a new branch based on your current HEAD |
| git checkout --track <remote/branch> | create a new tracking branch based on a remote branch |
| git merge [branch]| merge the specified branch's history into the current one|
| git add <resolved-file> or git rm <resolved-file>| editor to manually solve conflicts (after resolved mark as reolved)|
| git log --stat -M| show all commit logs with indication of any paths that may have moved|
| git log | show all commits in the current branch's history|
| git log -p <file>| show changes over time for a specific file|
| git blame <file> | who changed what and when in <file>|
| git rm [file] | delete the file from the project and stage the removal from commit|
| git mv [existing path] [new-path]| change an existing file path and stage the move
| rebase |
| git rebase <branch>| rebase your current HEAD onto <branch>|
| git rebase --abort | abort a rebase|
| git rebase --continue | continue a rebase after resolving conflicts|
| Update & Publish|
| git remote -v  | list all currently configured remotes |
| git remote show <remote>| show information about a remote |
| git remote add <shortname> <url> | add new remote repository, named <remote> |
| git fetch <remote> | download all changes from <remote> but don't integrate|
| git pull <remote> <branch>| download changes and directly merge/integrate into HEAD|
| git push <remote> <branch>| publish local changes on a remote |
| git branch -dr <remote/branch>| delete a branch on the remote |
| git push --tags|publish your tags |







