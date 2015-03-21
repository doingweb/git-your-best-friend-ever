## The Lifecycle of a File

Adding a file:

```
$ git status
On branch master
nothing to commit, working directory clean
$ atom new-file.txt
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        new-file.txt

nothing added to commit but untracked files present (use "git add" to track)
$ git add new-file.txt
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   new-file.txt

$ git commit -m "Added new file."
[master 015ba6c] Added new file.
 1 file changed, 1 insertion(+)
 create mode 100644 new-file.txt
$ git status
On branch master
nothing to commit, working directory clean
```

note:

During `atom new-file.txt`, I created the text file and added one line to it.
