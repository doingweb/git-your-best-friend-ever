## What's in a commit?

```
$ git cat-file -p 1eb2ce28cd1b6e89e9a9ed2f4681cb834a48fc87
tree 48b8b000be35eb9d739aa63b5556226405745e86
parent 8516b87e1307db03994c619693e2669a1d825608
author Chris Antes <chris@chrisdoingweb.com> 1426921898 -0700
committer Chris Antes <chris@chrisdoingweb.com> 1426921898 -0700

Slides on other VCSs. Refinements to previous slides.
```

```
$ git cat-file -p 48b8b000be35eb9d739aa63b5556226405745e86
100644 blob 69fad358018d530235f8e43c483d3ce960616a32    .bowerrc
100644 blob d1d8a4176a416daffcfbfecdd3f35f24bd79fc7d    .editorconfig
100644 blob 3518e7f29dcc2b195d7077d989efa3f6bd6cfbef    .gitignore
100644 blob 855a9efe0a6aff5c442fbd1dc26a5af279d66b72    .jshintrc
100644 blob 41ea8d4c4629041d42e6f090e41dcd3d5eace1eb    .yo-rc.json
100644 blob a62946614b7f1c3c43990b0cb39c2677060effc7    Gruntfile.coffee
100644 blob 6f7daeaa8cf04b03638ddd6509a2508efee2b5cd    bower.json
040000 tree c38c7e40dc6b3671486d99d2cc3a15c4a36cd604    css
040000 tree fc4a211f73968d6efb124f296f70acd9610eb19a    images
040000 tree 449df7430c1f8db1c0922d1fbc2ec99fb8ec3701    js
100644 blob 0eeb399333af39939d3c83691747f7cf30a002ee    package.json
040000 tree b938f6a0fd291522d106549360c0a7facdaf1f30    slides
040000 tree e4eaa88c5ddd86fd4a6a95bf2769d36565863dd8    templates
```

```
$ git cat-file -p 0eeb399333af39939d3c83691747f7cf30a002ee
{
  "name": "git-your-best-friend-ever",
  "version": "0.0.0",
  "private": true,
  "devDependencies": {
    "grunt": "^0.4.5",
    "grunt-autoprefixer": "^2.2.0",
    "grunt-coffeelint": "0.0.13",
    "grunt-contrib-connect": "^0.9.0",
    "grunt-contrib-copy": "^0.7.0",
    "grunt-contrib-jshint": "^0.10.0",
    "grunt-contrib-sass": "^0.8.0",
    "grunt-contrib-watch": "^0.6.1",
    "load-grunt-tasks": "^1.0.0"
  },
  "engines": {
    "node": ">=0.10.0",
    "npm": ">=1.3.7"
  },
  "scripts": {
    "test": "grunt test"
  }
}
```
