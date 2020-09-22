# *Gitflow Workflow*
 
**Gitflow Workflow** is a Git workflow design that was first published and made popular by Vincent Driessen at nvie. The Gitflow Workflow defines a **strict branching model** designed around the project release. This provides a robust framework for managing larger projects.  

Gitflow is ideally suited for projects that have a **scheduled release cycle**. It assigns very specific roles to different branches and defines how and when they should interact. In addition to feature branches, it uses individual branches for preparing, maintaining, and recording releases. Of course, you also get to leverage all the benefits of the Feature Branch Workflow: **pull requests, isolated experiments, and more efficient collaboration**.




# *How it works*

![working](https://wac-cdn.atlassian.com/dam/jcr:2bef0bef-22bc-4485-94b9-a9422f70f11c/02%20(2).svg?cdnVersion=1251)


## *Develop and Master Branches*
Instead of a single master branch, this workflow uses two branches to record the history of the project. The master branch stores the official release history, and the develop branch serves as an integration branch for features. It's also convenient to tag all commits in the master branch with a version number.

The first step is to complement the default master with a developed branch. A simple way to do this is for one developer to create an empty develop branch locally and push it to the server:

>git branch develop git push -u origin develop


This branch will contain the complete history of the project, whereas master will contain an abridged version. Other developers should now clone the central repository and create a tracking branch for develop.

When using the git-flow extension library, executing git flow init on an existing repo will create the develop branch:


>$ git flow init Initialized empty Git repository in ~/project/.git/ No branches exist yet. Base branches must be created now. Branch name for production releases: [master] Branch name for "next release" development: [develop]
>
>How to name your supporting branch prefixes? Feature branches? [feature/] Release branches? [release/] Hotfix branches? [hotfix/] Support branches? [support/] Version tag prefix? []
>
>$ git branch * develop  master***


# *Feature Branches*

Each new feature should reside in its own branch, which can be pushed to the central repository for backup/collaboration. But, instead of branching off of master, feature branches use develop as their parent branch. When a feature is complete, it gets merged back into develop. **Features should never interact directly with master**.

![feature_branches](https://wac-cdn.atlassian.com/dam/jcr:b5259cce-6245-49f2-b89b-9871f9ee3fa4/03%20(2).svg?cdnVersion=1251)

> Note that feature branches combined with the develop branch is, for all intents and purposes, the Feature Branch Workflow. But, the Gitflow Workflow doesn’t stop there.

Feature branches are generally created off to the latest develop branch.


## *Creating a feature branch*
 

Without the git-flow extensions:
 
>git checkout develop git checkout -b feature_branch


When using the git-flow extension:

>git flow feature start feature_branch

Continue your work and use Git like you normally would.


## *Finishing a feature branch*

When you’re done with the development work on the feature, the next step is to merge the feature_branch into develop.


Without the git-flow extensions:

>git checkout develop git merge feature_branch


Using the git-flow extensions:

>git flow feature finish feature_branch


# *Release Branches*

![how_to_release_branches](https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=1251)

Once develop has acquired enough features for a release (or a predetermined release date is approaching), you fork a release branch off of develop. Creating this branch starts the next release cycle, so no new features can be added after this point—only bug fixes, documentation generation, and other release-oriented tasks should go in this branch. Once it's ready to ship, the release branch gets merged into master and tagged with a version number. In addition, it should be merged back into develop, which may have progressed since the release was initiated.

Using a dedicated branch to prepare releases makes it possible for one team to polish the current release while another team continues working on features for the next release. It also creates well-defined phases of development.

Making release branches is another straightforward branching operation. Like feature branches, release branches are based on the develop branch. A new release branch can be created using the following methods.


Without the git-flow extensions:

>git checkout develop git checkout -b release/0.1.0


When using the git-flow extensions:

>$ git flow release start 0.1.0 Switched to a new branch 'release/0.1.0'


Once the release is ready to ship, it will get merged it into master and develop, then the release branch will be deleted. It’s important to merge back into develop.

To finish a release branch, use the following methods:

Without the git-flow extensions:

>git checkout master git merge release/0.1.0

Or with the git-flow extension:

>git flow release finish '0.1.0'


# *Hotfix Branches*

![hotfix_branches](https://wac-cdn.atlassian.com/dam/jcr:61ccc620-5249-4338-be66-94d563f2843c/05%20(2).svg?cdnVersion=1251)

**Maintenance or “hotfix” branches are used to quickly patch production releases.** Hotfix branches are a lot like release branches and feature branches except they're based on master instead of develop. This is the only branch that should fork directly off of master. As soon as the fix is complete, it should be merged into both master and develop (or the current release branch), and master should be tagged with an updated version number.

Having a dedicated line of development for bug fixes lets your team address issues without interrupting the rest of the workflow or waiting for the next release cycle. You can think of maintenance branches as ad hoc release branches that work directly with master. A hotfix branch can be created using the following methods:


Without the git-flow extensions:

>git checkout master git checkout -b hotfix_branch

When using the git-flow extensions: 

>$ git flow hotfix start hotfix_branch

Similar to finishing a release branch, a hotfix branch gets merged into both master and develop.

>git checkout master git merge hotfix_branch git checkout develop git merge hotfix_branch git branch -D hotfix_branch

>$ git flow hotfix finish hotfix_branch

# Example

A complete example demonstrating a Feature Branch Flow is as follows. Assuming we have a repo setup with a master branch.

>git checkout master
>
>git checkout -b develop
>
>git checkout -b feature_branch
>
>#work happens on feature branch
>
>git checkout develop
>
>git merge feature_branch
>
>git checkout master
>
>git merge develop
>
>git branch -d feature_branch>


# *Summary*

***The overall flow of Gitflow is:***

*1. A develop branch is created from master.*

*2. A release branch is created from develop.*

*3. Feature branches are created from develop.*

*4. When a feature is complete it is merged into the develop branch.*

*5. When the release branch is done it is merged into develop and master.*

*6. If an issue in master is detected a hotfix branch is created from master.*

*7. Once the hotfix is complete it is merged to both develop and master.*

