## Keeping Remotes Up-to-Date

Download new commits with `git fetch`:

<img alt="`git fetch origin` downloads missing commits from the `origin` remote." src="images/remote-branches-3.png" height="550">

note:

To integrate those upstream changes, you would then do a `git merge origin/master` (or `git rebase origin/master`) from the `master` branch. To do both steps in one, use [`git pull`](http://git-scm.com/book/en/v2/Git-Branching-Remote-Branches#Pulling).
