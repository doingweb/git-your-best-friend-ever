## Pushing a New Branch

Imagine we created a local branch and have now decided we want to track it, to make future pushes easier:

<pre><code data-trim data-noescape>
$ <span class="fragment">git checkout -b new-feature</span>
<span class="fragment">Switched to a new branch 'new-feature'
$</span> <span class="fragment">git push</span>
<span class="fragment">fatal: The current branch new-feature has no upstream branch.
To push the current branch and set the remote as upstream, use

   git push --set-upstream origin new-feature

$</span> <span class="fragment">git push --set-upstream origin new-feature</span>
<span class="fragment">Total 0 (delta 0), reused 0 (delta 0)
To git@github.com:doingweb/git-your-best-friend-ever.git
* [new branch]      new-feature -> new-feature
Branch new-feature set up to track remote branch new-feature from origin.
$</span> <span class="fragment">git push</span>
<span class="fragment">Everything up-to-date</span>
</code></pre>

note:

Tracking is automatically set up for branches that already exist on the remote.

Git is often very helpful, giving you copy-and-pastable commands right when you need them, saving you from having to go look them up.
