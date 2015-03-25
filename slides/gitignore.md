## `.gitignore`

```sh
# We want these files in our working directory, but not in our repository.

# Log files
*.log

# Build output directory
build/

# Third-party packages
node_modules
```

Matching files not already in the repository are ignored:

<pre><code data-trim data-noescape>
$ <span class="fragment">atom new-file-that-gets-ignored.log
$</span> <span class="fragment">git status</span>
<span class="fragment">On branch master
nothing to commit, working directory clean</span>
</code></pre>

note:

http://git-scm.com/docs/gitignore

For more ideas, check out [GitHub's repo of `.gitignore` templates](https://github.com/github/gitignore).
