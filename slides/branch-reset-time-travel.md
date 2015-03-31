## Time Travel with `git reset`

Resetting is useful when some commits should've been on a different branch:

<pre><code data-trim data-noescape>
$ <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean
$</span> <span class="fragment">git log --oneline</span>
<span class="fragment">4f00f1a Adding a few more cat names.
9abff09 Needed some cat names.
0d229e7 Removed the file.
9bb1e7e Modified the file.
015ba6c Added new file.
$</span> <span class="fragment">git branch feature/cat-names</span>
<span class="fragment">$</span> <span class="fragment">git reset --hard HEAD~2</span>
<span class="fragment">HEAD is now at 0d229e7 Removed the file.
$</span> <span class="fragment">git checkout feature/cat-names</span>
<span class="fragment">Switched to branch 'feature/cat-names'
$</span> <span class="fragment">git log --oneline</span>
<span class="fragment">4f00f1a Adding a few more cat names.
9abff09 Needed some cat names.
0d229e7 Removed the file.
9bb1e7e Modified the file.
015ba6c Added new file.</span>
</code></pre>

note:

This has happened to me on numerous occasions.
