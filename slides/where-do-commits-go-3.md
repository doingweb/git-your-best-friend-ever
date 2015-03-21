## Where do commits go?

Commits live in the *key-value store* (`.git/objects` directory):

```
$ ls -R .git/objects
.git/objects:
1e  5e  ce  info  pack

.git/objects/1e:
b98e70230c45fa1b61eab232ec1f66b29c8625

.git/objects/5e:
08bc4c2da476233573fc7c4793412cede36bfa

.git/objects/ce:
013625030ba8dba906f756967f9e9ca394464a

.git/objects/info:

.git/objects/pack:

```

note:

This is from a repository with a single commit of a single file, not packed. The key-value store of a repository any larger than that wouldn't fit so nicely on a slide.
