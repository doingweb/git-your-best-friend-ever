## Deleting Branches

Delete branches with `git branch --delete`:

<pre><code data-trim data-noescape>
$ <span class="fragment">git branch --list</span>
<span class="fragment">* master
  new-feature
$</span> <span class="fragment">git branch --delete new-feature</span>
<span class="fragment">Deleted branch new-feature (was f3bc86a).
$</span> <span class="fragment">git branch --list</span>
<span class="fragment">* master</span>
</code></pre>

note:

This doesn't actually delete any commits! It only deletes the branch, which is just a pointer to a commit. However, if that branch was the only reference to its commit, then a [garbage collection](http://git-scm.com/docs/git-gc) will end up deleting the commit, since it is unreferenced. This command reports the hash of the deleted branch's commit to give you the opportunity to create a reference to the now potentially unreferenced commit.
