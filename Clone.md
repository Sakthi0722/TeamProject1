# Clone

When you create a repository on your GitHub Enterprise Server instance, it exists as a remote repository. You can clone your repository to create a local copy on your computer and sync between the two locations.

You can clone a repository from GitHub to your local computer to make it easier to fix merge conflicts, add or remove files, and push larger commits. When you clone a repository, you copy the repository from GitHub to your local machine.Cloning a repository pulls down a full copy of all the repository data that GitHub has at that point in time, including all versions of every file and folder for the project. You can push your changes to the remote repository on GitHub, or pull other people's changes from GitHub.
## How to Clone
1. On GitHub Enterprise, navigate to the main page of the repository.
![Image1](Images\Image9.png "Image1")
2. Under the repository name, click Clone or download.
![Image1](Images\Image8.png "Image2")
3. In the Clone with HTTPs section, click copy the clone URL for the repository.
  
4. Open Git Bash/Webstorm/Anything you Wish. In this we use Git Bash.

5. Change the current working directory to the location where you want the cloned directory to be made.
 
6. Type **git clone**, and then paste the URL you copied in Step 2.

7. Press Enter. Your local clone will be created.
![Image1](Images\Image7.png "Image3")  
