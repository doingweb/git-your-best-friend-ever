## What's in a commit?

<img src="images/commit-and-tree.png" alt="A commit contains a pointer to a tree, and trees point to a collection of blobs and/or other trees." height="600">

note:

Commits, trees, and blobs are all stored together in the key-value store.

If a file hasn't changed, the tree of the new commit will just re-use the previous blob. If the file *has* changed, Git will create a new blob for the file. That might sound kind of space-inefficient, but 1) space is cheaper than time, and not having to rebuild files from deltas saves a lot of time, 2) all objects in the store are compressed with [zlib](http://en.wikipedia.org/wiki/Zlib), and 3) [packing does a bunch of things](http://git.kernel.org/cgit/git/git.git/tree/Documentation/technical/pack-heuristics.txt?id=HEAD) to save space.
