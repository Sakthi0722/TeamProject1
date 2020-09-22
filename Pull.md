# *PULL*

![pull](https://static.javatpoint.com/tutorial/git/images/git-pull.png)

The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo.


> git pull [options] [repository [refspec...]]


## *Example*

- Update the remote-tracking branches for the repository you cloned from, then merge one of them into your current branch:

> $ git pull
>
> $ git pull origin

- Merge into the current branch the remote branch next:

> $ git pull origin next

This leaves a copy of next temporarily in FETCH_HEAD, and updates the remote-tracking branch origin/next. The same can be done by invoking fetch and merge:

> $ git fetch origin
>
> $ git merge origin/next

*NOTE: If you tried a pull which resulted in complex conflicts and would want to start over, you can recover with git reset.*
