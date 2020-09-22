# *PUSH*


The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo.


>git push [remote] [branch]

## *Before Pushing*
![before_pushing](https://wac-cdn.atlassian.com/dam/jcr:f148974e-7d4d-4c0e-bd31-8ac5467d1e6a/04.svg?cdnVersion=1253)
## *After Pushing*
![after_pushing](https://wac-cdn.atlassian.com/dam/jcr:f148974e-7d4d-4c0e-bd31-8ac5467d1e6a/04.svg?cdnVersion=1253)

## *Example*

The following example describes one of the standard methods for publishing local contributions to the central repository. First, it makes sure your local master is up-to-date by fetching the central repository’s copy and rebasing your changes on top of them. The interactive rebase is also a good opportunity to clean up your commits before sharing them. Then, the git push command sends all of the commits on your local master to the central repository.

>git checkout master
>
>git fetch origin master
>
>git rebase -i origin/master
>
>git push origin master
