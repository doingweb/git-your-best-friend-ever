## What's in a commit?

Let's see what a blob looks like:

<pre><code data-trim data-noescape>
$ <span class="fragment">git cat-file -p 0eeb399333af39939d3c83691747f7cf30a002ee</span>
<span class="fragment">{
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
}</span>
</code></pre>

note:

This is exactly the content of the file I had on disk when I made this commit.
