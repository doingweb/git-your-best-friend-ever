## Renaming Branches

Branches can be renamed with `git branch --move`:

<pre><code data-trim data-noescape>
$ <span class="fragment">git branch --list</span>
<span class="fragment">  master
* new-feature
$</span> <span class="fragment">git branch --move new-feature feature/starring-items</span>
<span class="fragment">$</span> <span class="fragment">git branch --list</span>
<span class="fragment">* feature/starring-items
  master</span>
</code></pre>

note:

Here we rename a very generically-named feature branch to something more helpful (and logically organized).

Also notice that branches are sorted by name. This reinforces that there's nothing inherently special about the `master` branch.
