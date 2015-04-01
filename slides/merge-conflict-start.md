## Merge Conflicts Happen

Let's say I did some similar work on two branches that I now want to merge:

<pre><code data-trim data-noescape>
$ <span class="fragment">git merge feature/cat-names</span>
<span class="fragment">Auto-merging cat-names.txt
CONFLICT (add/add): Merge conflict in cat-names.txt
Automatic merge failed; fix conflicts and then commit the result.
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
You have unmerged paths.
  (fix conflicts and run "git commit")

Unmerged paths:
  (use "git add <file>..." to mark resolution)

        both added:      cat-names.txt

no changes added to commit (use "git add" and/or "git commit -a")
</code></pre>

<p class="fragment">So scary!</p>
