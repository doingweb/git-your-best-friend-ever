## The Lifecycle of a File

Modifying a file:

<pre><code data-trim data-noescape>
$ <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean
$</span> <span class="fragment">atom new-file.txt
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   new-file.txt

no changes added to commit (use "git add" and/or "git commit -a")
$</span> <span class="fragment">git add new-file.txt
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   new-file.txt

$</span> <span class="fragment">git commit -m "Modified the file."</span>
<span class="fragment">[master 9bb1e7e] Modified the file.
 1 file changed, 1 insertion(+)
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean</span>
</code></pre>

note:

During `atom new-file.txt`, I added a line to the text file.

`git checkout` copies files from a given tree into the working directory, as implied by the earlier slide. If a branch or commit is specified, it'll get that tree from the repository and also update the `HEAD` to point to it. If `--` is specified, it'll get the tree from the index.

This and the previous (adding the file) commit report `1 insertion(+)` because the change I made in both of those instances was to add a line of text.
