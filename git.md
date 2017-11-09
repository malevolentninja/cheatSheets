


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
















