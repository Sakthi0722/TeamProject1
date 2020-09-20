# Introduction to Git
Git is an **Open Source Distributed Version Control System**.This basically means that Git is a content tracker. So Git can be used to store content. The code which is stored in Git keeps changing as more code is added. Also, many developers can add code in parallel. So Version Control System helps in handling this by maintaining a history of what changes have happened.<br />

**Distributed Version Control System**: Git has a remote repository which is stored in a server, and a local repository which is stored on the computer of each developer. This means that the code is not just stored in a central server, but the full copy of the code is present in all the developers’ computers. Git is a Distributed Version Control System since the code is present in every developer’s computer.

## Repository
A repository, or Git project, encompasses the entire collection of files and folders associated with a project, along with each file’s revision history. The file history appears as snapshots in time called commits, and the commits exist as a linked-list relationship, and can be organized into multiple lines of development called branches. Because Git is a DVCS, repositories are self-contained units and anyone who owns a copy of the repository can access the entire codebase and its history. Using the command line or other ease-of-use interfaces, a git repository also allows for: interaction with the history, cloning, creating branches, committing, merging, comparing changes across versions of code, and more.

Working in repositories keeps development projects organized and protected. Developers are encouraged to fix bugs, or create fresh features, without fear of derailing mainline development efforts. Git facilitates this through the use of topic branches: lightweight pointers to commits in history that can be easily created and deprecated when no longer needed.Through platforms like GitHub, Git also provides more opportunities for project transparency and collaboration. Public repositories help teams work together to build the best possible final product.


## Basic Git commands 
To use Git, developers use specific commands to copy, create, change, and combine code. These commands can be executed directly from the command line or by using an application like GitHub Desktop or Git Kraken. Here are some common commands for using Git:
                        
**git init** initializes a brand-new Git repository and begins tracking an existing directory. It adds a hidden sub folder within the existing directory that houses the internal data structure required for version control.

**git clone** creates a local copy of a project that already exists remotely. The clone includes all the project’s files, history, and branches.

**git add** stages a change. Git tracks changes to a developer’s codebase, but it’s necessary to stage and take a snapshot of the changes to include them in the project’s history. This command performs staging, the first part of that two-step process. Any changes that are staged will become a part of the next snapshot and a part of the project’s history. Staging and committing separately gives developers complete control over the history of their project without changing how they code and work.

**git commit** saves the snapshot to the project history and completes the change-tracking process. In short, a commit functions like taking a photo. Anything that’s been staged with git add will become a part of the snapshot with git commit.

**git status** shows the status of changes as untracked, modified, or staged.

**git branch** shows the branches being worked on locally.

**git merge** merges lines of development together. This command is typically used to combine changes made on two distinct branches. For example, a developer would merge when they want to combine changes from a feature branch into the main branch for deployment.

**git pull** updates the local line of development with updates from its remote counterpart. Developers use this command if a teammate has made commits to a branch on a remote, and they would like to reflect those changes in their local environment.

**git push** updates the remote repository with any commits made locally to a branch.

## Git vs GitHub
**Git** is a version control system that lets you manage and keep track of your source code history. **GitHub** is a cloud-based hosting service lets you manage Git repositories. If you have open-source projects that use Git, then GitHub is designed to help you better manage them.
