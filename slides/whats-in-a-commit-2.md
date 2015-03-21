## What's in a commit?

Let's go look at a raw commit!

`git cat-file` gets objects from the key-value store:

```
$ git cat-file -p 1eb2ce28cd1b6e89e9a9ed2f4681cb834a48fc87
tree 48b8b000be35eb9d739aa63b5556226405745e86
parent 8516b87e1307db03994c619693e2669a1d825608
author Chris Antes <chris@chrisdoingweb.com> 1426921898 -0700
committer Chris Antes <chris@chrisdoingweb.com> 1426921898 -0700

Slides on other VCSs. Refinements to previous slides.
```

note:

We use `git cat-file`, because the actual object files stored on disk are [compressed and specially-formatted](http://git-scm.com/book/en/v2/Git-Internals-Git-Objects#Object-Storage).

The commit we're looking at is the last commit in the log from a few slides ago.

The `-p` on `git cat-file` makes it print nicely.