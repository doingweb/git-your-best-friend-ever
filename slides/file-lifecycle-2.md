## The Lifecycle of a File

Adding a file:

<pre><code data-trim data-noescape>
$ <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean
$</span> <span class="fragment">atom new-file.txt
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        new-file.txt

nothing added to commit but untracked files present (use "git add" to track)
$</span> <span class="fragment">git add new-file.txt
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   new-file.txt

$</span> <span class="fragment">git commit -m "Added new file."</span>
<span class="fragment">[master 015ba6c] Added new file.
 1 file changed, 1 insertion(+)
 create mode 100644 new-file.txt
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean</span>
</code></pre>

note:

During `atom new-file.txt`, I created the text file and added one line to it.

`git add` takes the given file in the working directory and adds it to the index, staging it for commit.

`git reset` resets the index to the given commit (optionally only for the given file).
