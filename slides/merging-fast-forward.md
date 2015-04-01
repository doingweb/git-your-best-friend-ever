## Fast-Forward Merges

<pre><code data-trim data-noescape>
$ <span class="fragment" data-fragment-index="1">git checkout master</span>
<span class="fragment" data-fragment-index="2">Switched to branch 'master'
$</span> <span class="fragment" data-fragment-index="3">git merge hotfix</span>
<span class="fragment" data-fragment-index="4">Updating f42c576..3a0874c
Fast-forward
 index.html | 2 ++
 1 file changed, 2 insertions(+)</span>
</code></pre>

<div style="position: relative; overflow: hidden;">
    <img alt="A commit timeline with a `hotfix` branch ahead of `master` by one commit." src="images/basic-branching-4.png" style="width: 680px; margin: 96px auto 0 auto;" class="fragment fade-out" data-fragment-index="4">
    <img alt="A commit timeline showing the `master` and `hotfix` branches now pointing at the same commit." src="images/basic-branching-5.png" style="position: absolute; width: 680px; left: 50%; margin-left: -340px; top: 0;" class="fragment" data-fragment-index="4">
</div>

note:

Git will fast-forward by default, where possible. 
