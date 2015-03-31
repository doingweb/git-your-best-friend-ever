## Changing Where a Branch Points

`git reset` changes where the `HEAD` branch points. And maybe some other stuff:

<div>
    <div style="width: 650px; margin: 0 auto; position: relative;">
        <img data-fragment-index="1" src="images/reset-start.png" alt="No reset commands have been run. `file.txt` is at version 3 in the `HEAD` commit, index, and working directory." class="fragment fade-out">
        <img data-fragment-index="1" src="images/reset-soft.png" alt="`git reset --soft HEAD~` is executed, which moves the `HEAD` branch (`master`) back by one commit (`file.txt` at version 2), but the index and working directory remain the same, both containing version 3." class="fragment current-visible" style="position: absolute; width: 100%; left: 16px;">
        <img src="images/reset-mixed.png" alt="`git reset --mixed HEAD~` is executed, which moves the `HEAD` branch (`master`) back by one commit and changes the index copy of `file.txt` back to version 2. The working directory copy is still at version 3." class="fragment current-visible" style="position: absolute; width: 100%; left: 16px;">
        <img src="images/reset-hard.png" alt="`git reset --hard HEAD~` is executed, which moves the `HEAD` branch (`master`) back by one commit, and brings the index and working directory copies of `file.txt` back to version 2." class="fragment" style="position: absolute; width: 100%; left: 16px;">
    </div>
</div>

note:

`HEAD~` is short for `HEAD~1`. `HEAD~2` would go back two commits. The [tilde and caret operators](http://www.paulboxley.com/blog/2011/06/git-caret-and-tilde) are useful tools for referring to commits navigable from the HEAD commit.

`git reset --soft HEAD~` followed by a `git commit` is similar to a `git commit --amend`; you're effectively re-doing your last commit. You can *squash* multiple commits together in this way, by specifying more than one traversal (e.g., `HEAD~2`). Note that, like `git commit --amend`, resetting and committing like this also **alters history**!

http://git-scm.com/docs/git-reset
