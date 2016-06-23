Git Basics
==========

| TOC
| Environment
| Experiment
| Creating Repositories
| Git Beginning
| 


Git is a DVCS (Distributed Version Control System). 'Version Control System'
means it saves history of different versions of your files, and 'Distributed'
means that there is no single point of failure like central server or repository
and instead every participant has a full copy of all files. 

Git was invented by Linus Torvalds, an unpleasant and contemptible person, which
is reflected in the name of the program.

Simply put Git is a tool to send patches over electrical mail. Git is a
collection of specialized tools for solving particular problems, problems you
might not really need to solve.

Commit
------

A commit is a patch. It describes modifications made to some files using 'diff'
format. 

A patch shows *differences* between two groups of files(two trees as in file
system hierarchy).

Git commit codifies where a patch should be applied. 

Git history is a long chain of instructions for recreating code base from the
beginning, step by step.

Commit C: My parent - B. Append "three" to the "numbers.txt".
Commit B: My parent - A. Append "two" to the "numbers.txt".
Commit A: Create file "numbers.txt" containing "one".

Commit A has no parent so it can only create new files, there are no files to
modify. Otherwise it is the same as any other commit.

So you start from a blank page. Then you apply patch A, which creates one. Then
you can apply patch B, which appends two, creating "one two", then you can apply
patch C to create "one two three".

A-->B-->C

Branches
--------

To create a patch to some code you need to have an original copy of code. You
use branches to create that copy, then you work on it, and when you ready you
can merge the code with your original safely.

Branches allow history to be non-linear, you can have several parallel branches
and merge/fork them however you want.

Remote repository
-----------------

Remote repository is just a repository that is located somewhere else. It can be
a central server, or your friend's computer.

Merging
-------


