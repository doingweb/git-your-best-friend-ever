## It's just a directory!

![A .git folder open in Windows Explorer](images/git-directory.png)

note:

Many of these files are **plain text**, and some of them are **editable**:

- `config`
- `hooks/*`
- `description`
- `info/exclude`

You'll probably want to use Git commands to manipulate the others.

The `objects` directory contains [the key-value store](http://git-scm.com/book/en/v2/Git-Internals-Git-Objects). Objects (commits, trees, blobs) can be read out of it using `git cat-file -p *[object hash]*`.

When you connect to a remote repository, this is the directory on the remote that you reference.

A "bare" repository is a repository made up of just this directory (no working directory).
