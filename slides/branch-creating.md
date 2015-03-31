## Creating Branches

Create new branches with `git branch`:

<pre><code data-trim data-noescape>
$ <span class="fragment" data-fragment-index="1">git branch --list</span>
<span class="fragment" data-fragment-index="2">* master
$</span> <span class="fragment" data-fragment-index="3">git branch new-feature</span>
<span class="fragment" data-fragment-index="4">$</span> <span class="fragment" data-fragment-index="5">git branch --list</span>
<span class="fragment" data-fragment-index="6">* master
  new-feature</span>
</code></pre>

<p class="fragment" data-fragment-index="7">Use `git checkout` to branch and switch in one command:</p>

<pre class="fragment" data-fragment-index="7"><code data-trim data-noescape>
$ <span class="fragment" data-fragment-index="8">git branch --list</span>
<span class="fragment" data-fragment-index="9">* master
$</span> <span class="fragment" data-fragment-index="10">git checkout -b new-feature</span>
<span class="fragment" data-fragment-index="11">Switched to a new branch 'new-feature'
$</span> <span class="fragment" data-fragment-index="12">git branch --list</span>
<span class="fragment" data-fragment-index="13">  master
* new-feature</span>
</code></pre>

note:

The `new-feature` branch being created in both scenarios is just another pointer to the same commit pointed to by `master` (since that's the `HEAD` when we create the new branch).

I recommend playing with these branch management commands in [Peter Cottle's LearnGitBranching](pcottle.github.io/learnGitBranching/?NODEMO) to get the hang of them in a more visual environment.
