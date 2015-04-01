## What's `HEAD`?

`HEAD` is just a pointer to the current branch.

<pre><code data-trim data-noescape>
$ <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean
$</span> <span class="fragment">cat .git/HEAD</span>
<span class="fragment">ref: refs/heads/master</span>
</code></pre>
