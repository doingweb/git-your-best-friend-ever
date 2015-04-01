## Rebasing

Replay commits as if you had based them off of a different commit:

<pre><code data-trim data-noescape>
$ <span class="fragment" data-fragment-index="1">git checkout experiment</span>
<span class="fragment" data-fragment-index="2">$</span> <span class="fragment" data-fragment-index="3">git rebase master</span>
<span class="fragment" data-fragment-index="4">First, rewinding head to replay your work on top of it...
Applying: added staged command</span>
</code></pre>

<div style="position: relative; overflow: hidden;">
    <img alt="A commit timeline with diverged `experiment` and `master` branches." src="images/basic-rebase-1.png" style="width: 880px; margin: 0 auto;" class="fragment fade-out" data-fragment-index="4">
    <img alt="A commit timeline showing an `experiment` branch one (rebased) commit ahead of `master`." src="images/basic-rebase-3.png" style="position: absolute; width: 1080px; left: 50%; margin-left: -540px; top: 0;" class="fragment" data-fragment-index="4">
</div>

note:

**This changes history!**

Rebasing is really nice for keeping noisy merge commits to a minimum when you need to continually integrate upstream changes, but can cause a lot of problems for teammates if they base work off of commits that get thrown out by a rebase. Communicate or don't do it!

http://git-scm.com/book/en/v2/Git-Branching-Rebasing#Rebase-vs.-Merge
