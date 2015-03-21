## The Lifecycle of a File

Removing a file:

```
$ git status
On branch master
nothing to commit, working directory clean
$ git rm new-file.txt
rm 'new-file.txt'
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        deleted:    new-file.txt

$ git commit -m "Removed the file."
[master 0d229e7] Removed the file.
 1 file changed, 2 deletions(-)
 delete mode 100644 new-file.txt
$ git status
On branch master
nothing to commit, working directory clean
```
