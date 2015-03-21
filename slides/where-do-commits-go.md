## Where do commits go?

![A singly-linked list of commits, arrows pointing in reverse chronological order.](images/commits-and-parents.png)

note:

We're going to get technical for a few minutes.

In terms of the data structure, new commits are added to the end of a singly-linked list representing the history of the repository.

"Snapshots" here represent the files for the commit (reflected in the working directory).
