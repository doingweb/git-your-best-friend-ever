## Merge Conflicts: Not Really Scary

Here's what the conflicted file looks like:

<pre><code data-trim data-noescape>
<span class="fragment burn current-visible" data-fragment-index="1"><<<<<<< HEAD</span>
<span class="fragment burn current-visible" data-fragment-index="2">Fluffy
Socrates</span>
<span class="fragment burn current-visible" data-fragment-index="1">=======</span>
<span class="fragment burn current-visible" data-fragment-index="3">Halo-Halo
Chairman Meow</span>
<span class="fragment burn current-visible" data-fragment-index="1">>>>>>>> feature/cat-names</span>
<span class="fragment burn current-visible" data-fragment-index="4">Sadie
Whiskers
Simba</span>
</code></pre>

<ul>
    <li class="fragment" data-fragment-index="1">The `<<<<<<<`, `=======`, and `>>>>>>>` lines denote where the conflict(s) are.</li>
    <li class="fragment" data-fragment-index="2">The `HEAD` section is what *our* file (what we're merging into) has.</li>
    <li class="fragment" data-fragment-index="3">The other section is what *their* file (what we're merging from) has.</li>
    <li class="fragment" data-fragment-index="4">The rest of the file has been merged automatically.</li>
</ul>
