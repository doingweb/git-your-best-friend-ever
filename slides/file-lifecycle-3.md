## The Lifecycle of a File

Modifying a file:

```
$ git status
On branch master
nothing to commit, working directory clean
$ atom new-file.txt
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   new-file.txt

no changes added to commit (use "git add" and/or "git commit -a")
$ git add new-file.txt
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   new-file.txt

$ git commit -m "Modified the file."
[master 9bb1e7e] Modified the file.
 1 file changed, 1 insertion(+)
$ git status
On branch master
nothing to commit, working directory clean
```

note:

During `atom new-file.txt`, I added a line to the text file.
