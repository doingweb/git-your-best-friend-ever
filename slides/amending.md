## Amending a Commit

Redo commits with `git commit --amend`:

<pre><code data-trim data-noescape>
$ <span class="fragment">git log --oneline --max-count 2</span>
<span class="fragment">0d229e7 Removed the file.
9bb1e7e Modified the file.
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   cat-names.txt

$</span> <span class="fragment">git commit -m "Needed soem cat names."</span>
<span class="fragment">[master 2e6c3b7] Needed soem cat names.
 1 file changed, 1 insertion(+)
 create mode 100644 cat-names.txt
$</span> <span class="fragment">git log --oneline --max-count 2</span>
<span class="fragment">2e6c3b7 Needed soem cat names.
0d229e7 Removed the file.
$</span> <span class="fragment">git commit --amend -m "Needed some cat names."</span>
<span class="fragment">[master c86eff7] Needed some cat names.
 1 file changed, 1 insertion(+)
 create mode 100644 cat-names.txt
$</span> <span class="fragment">git log --oneline --max-count 2</span>
<span class="fragment">c86eff7 Needed some cat names.
0d229e7 Removed the file.</span>
</code></pre>

<span class="fragment">Note that **this changes history**!</span>

note:

The `--amend` option lets you alter the most recent commit. Staged changes are included and you have the opportunity to change the message (perhaps to fix a spelling mistake, as seen here).

Be aware that amending a commit is one of the [Git commands that rewrite history](http://git-scm.com/book/en/v2/Git-Tools-Rewriting-History), and it must be used with care when collaborating with others. If you push a commit that later gets amended and someone else bases work on it, they'll have to manually correct it. This is one big place where good team policies and communication will save everyone a lot of time and frustration.
