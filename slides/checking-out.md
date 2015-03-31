## Switching Branches

Switch branches with `git checkout`:

<pre><code data-trim data-noescape>
$ <span class="fragment" data-fragment-index="1">git branch --list</span>
<span class="fragment" data-fragment-index="2">* master
  testing
$</span> <span class="fragment" data-fragment-index="3">git checkout testing</span>
<span class="fragment" data-fragment-index="4">Switched to branch 'testing'</span>
</code></pre>

<div>
    <div style="width: 500px; margin: 0 auto; position: relative;">
        <img data-fragment-index="4" src="images/head-to-master.png" alt="`HEAD` points to the `master` branch." class="fragment fade-out">
        <img data-fragment-index="4" src="images/head-to-testing.png" alt="`HEAD` now points to the `testing` branch." class="fragment" style="position: absolute; left: 12px; top: 82px;">
    </div>
</div>

note:

Checking out a branch also updates the index and working directory. A plain checkout (i.e., not a [`--force` or `--merge` checkout](http://git-scm.com/docs/git-checkout)) will prevent data loss by failing if there are any conflicts with uncommitted changes.
