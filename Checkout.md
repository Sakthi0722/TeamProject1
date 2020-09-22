# *CHECKOUT*

![checkout](https://static.javatpoint.com/tutorial/git/images/git-checkout.png)
Updates files in the working tree to match the version in the index or the specified tree. If no pathspec was given, git checkout will also update HEAD to set the specified branch as the current branch.


>git checkout [branch]

To prepare for working on branch, switch to it by updating the index and the files in the working tree, and by pointing HEAD at the branch. Local modifications to the files in the working tree are kept, so that they can be committed to the <branch>.

## *Example*

The following sequence checks out the master branch, reverts the Makefile to two revisions back, deletes hello.c by mistake, and gets it back from the index.

> $ git checkout master
>
> $ git checkout master~2 Makefile
>
> $ rm -f hello.c
>
> $ git checkout hello.c

1. switch branch
2. take a file out of another commit
3. restore hello.c from the index
