## Cloning a Remote

Cloning is the first step to working with an existing repository:

<img alt="`master` and `origin/master` branches are created as a result of a `git clone`." src="images/remote-branches-1.png" height="550">

note:

The remote URL gets stored away in `.git/config`, along with some other metadata about the connection.

Remote branches are branches, too! They are made of the same stuff, at least -- the `master` branch file (containing its commit hash) is `.git/refs/heads/master`, and the `origin/master` file is `.git/refs/remotes/origin/master`.

The name `origin` isn't special, other than the fact that it's the default remote name. Just like `master` is with branches.

Remote branches aren't *exactly* like local (*head*) branches. They're meant to represent the state of another repository, so they can't be altered directly. They cannot be checked out (or therefore committed to) or reset. They can, however, be merged from or rebased onto.
