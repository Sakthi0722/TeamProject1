# *REMOTE ADD/ REMOVE/ SHOW*

![remote](https://wac-cdn.atlassian.com/dam/jcr:df13d351-6189-4f0b-94f0-21d3fcd66038/01.svg?cdnVersion=1253)

It manages the set of repositories ("remotes") whose branches you track.

> git remote



## *Example*

- *add*

Adds a remote named [name] for the repository at [url]. The command git fetch <name> can then be used to create and update remote-tracking branches [name]/[branch].

>$ git remote add origin https://github.com/user/repo.git (set a new remote)
>
> $ git remote -v (Verify new remote)
>
> origin  https://github.com/user/repo.git (fetch)
>
> origin  https://github.com/user/repo.git (push)

- *remove*

If you want to remove a remote for some reason - you’ve moved the server or are no longer using a particular mirror, or perhaps a contributor isn’t contributing anymore — you can either use git remote remove or git remote rm:

> $ git remote remove paul
>
>$ git remote
>
>origin

- *show*

Invoking git remote with the -v option will print the list of bookmarked repository names and additionally, the corresponding repository URL. The -v option stands for "verbose". Below is example output of verbose git remote output.

> git remote -v
>
> origin  git@bitbucket.com:origin_user/reponame.git (fetch)
>
> origin  git@bitbucket.com:origin_user/reponame.git (push)
>
> upstream    https://bitbucket.com/upstream_user/reponame.git (fetch)
>
> upstream    https://bitbucket.com/upstream_user/reponame.git (push)
>
> other_users_repo    https://bitbucket.com/other_users_repo/reponame (fetch)
>
> other_users_repo    https://bitbucket.com/other_users_repo/reponame (push)
