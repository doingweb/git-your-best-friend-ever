## Resolving Conflicts

Once we've manually merged our conflicted files, we use `git add` to tell Git that we've resolved the conflicts, then we resume the merge commit with `git commit`:

<pre><code data-trim data-noescape>
$</span> <span class="fragment">git add cat-names.txt</span>
<span class="fragment">$</span> <span class="fragment">git commit</span>
<span class="fragment">[master b98a343] Merge branch 'feature/cat-names'</span>
</code></pre>

note:

Since we were already in the middle of a merge, `git commit` will open the text editor with the default merge commit message (which, in this case, also includes a note about the conflicts). Simply quitting the editor completes the commit.
