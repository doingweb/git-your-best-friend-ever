## Where do commits go?

Commits live in the *key-value store* (`.git/objects` directory):

<pre><code data-trim data-noescape>
$ <span class="fragment">ls -R .git/objects</span>
<span class="fragment">.git/objects:
1e  5e  ce  info  pack

.git/objects/1e:
b98e70230c45fa1b61eab232ec1f66b29c8625

.git/objects/5e:
08bc4c2da476233573fc7c4793412cede36bfa

.git/objects/ce:
013625030ba8dba906f756967f9e9ca394464a

.git/objects/info:

.git/objects/pack:
</span>
</code></pre>

note:

[SHA-1](http://en.wikipedia.org/wiki/SHA-1) hashes are used as keys for the objects. This guarantees that the contents of those objects are correct (and, implicitly, references between objects), protecting the entire history from undetected corruption.

The full 40-character hash of the first object listed above is `1eb98e70230c45fa1b61eab232ec1f66b29c8625`. Git stores the objects in folders named with the first two characters, then in files named with the remaining 38. This helps divide up the thousands of object files that can accumulate over time.

This is from a repository with a single commit of a single file, not [packed](http://git-scm.com/book/en/v2/Git-Internals-Packfiles). The key-value store of a repository any larger than that wouldn't fit so nicely on a slide.
