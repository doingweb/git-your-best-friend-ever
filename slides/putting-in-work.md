## Putting In Work

<img src="images/areas.png" alt="When a commit is checked out, the working directory is updated with those commit's files. After some changes are made, those changes are staged and then subsequently committed to the repository." height="625">

note:

The working directory is initialized with files from a commit, changes are made, staged, then committed.

The *Staging* area is a data structure (also known as the *index*, stored in `.git/index`) that holds the `tree` object for the next commit. When the working directory is clean, it is the same as the `HEAD` commit. As files are added and removed, those changes are reflected in the index.
