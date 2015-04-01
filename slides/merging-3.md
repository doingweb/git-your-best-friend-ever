## Merging Branches

<pre><code data-trim data-noescape>
$ <span class="fragment">git checkout master</span>
<span class="fragment">Switched to branch 'master'
$</span> <span class="fragment">git merge iss53</span>
<span class="fragment">Merge made by the 'recursive' strategy.
index.html |    1 +
1 file changed, 1 insertion(+)</span>
</code></pre>

<div class="fragment" style="overflow: hidden;">
    <img alt="A commit timeline with an `iss53` branch merged into `master`. The new merge commit, C6, has two parents, C4 from `master` and C5 from `iss53`." src="images/basic-merging-2.png" height="500" style="margin-top: -80px;">
</div>
