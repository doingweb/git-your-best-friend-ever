## Other Really Useful Git Commands

I don't use these every day, but they're just so nice to have when you need them:

### `git log --grep="search terms"`

Searches commit messages. Accepts regular expressions.

### `git stash`

Saves the working directory changes onto a stack, so you can switch branches without having to commit. `git stash pop` applies the topmost changes and removes them from the stack.

### `git bisect`

Perform a binary search for the commit that introduced a bug.

note:

 * http://git-scm.com/docs/git-log
 * http://git-scm.com/book/en/v1/Git-Tools-Stashing
 * http://git-scm.com/docs/git-bisect
