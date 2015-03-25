## The Lifecycle of a File

Removing a file:

<pre><code data-trim data-noescape>
$ <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean
$</span> <span class="fragment">git rm new-file.txt</span>
<span class="fragment">rm 'new-file.txt'
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        deleted:    new-file.txt

$</span> <span class="fragment">git commit -m "Removed the file."</span>
<span class="fragment">[master 0d229e7] Removed the file.
 1 file changed, 2 deletions(-)
 delete mode 100644 new-file.txt
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean</span>
</code></pre>
