Required Commands

ls - used to list files and directories
mkdir - used to create a new directory
cd - used to change directories
rm - used to remove files and directories
pwd - print working directory


mkdir -p udacity-git-course/new-git-project && cd $_ - to get inside the  new-git-project directory

Git Init's Effect		
Running the git init command sets up all of the necessary files and directories that Git will use to keep 
track of everything. All of these files are stored in a directory called .git (notice the . at the beginning - that 
means it'll be a hidden directory on Mac/Linux). This .git directory is the "repo"! This is where git records all of the commits and keeps track of everything!

Let's take a brief look at the contents of the .git directory.

WARNING: Don't directly edit any files inside the .git directory. This is the heart of the repository. 
If you change file names and/or file content, git will probably lose track of the files that you're 
keeping in the repo, and you could lose a lot of work! It's okay to look at those files though, but don't edit or delete them.


.Git Directory Contents
We're about to take a look at the .git directory...it's not vital for this course, though, so don't worry about memorizing anything, 
it's here if you want to dig a little deeper into how Git works under the hood.

Here's a brief synopsis on each of the items in the .git directory:

config file - where all project specific configuration settings are stored.
From the Git Book(opens in a new tab):
Git looks for configuration values in the configuration file in the Git directory (.git/config) of whatever repository 
you’re currently using. These values are specific to that single repository.

For example, let's say you set that the global configuration for Git uses your personal email address. 
If you want your work email to be used for a specific project rather than your personal email, that change would be added to this file.

description file - this file is only used by the GitWeb program, so we can ignore it

hooks directory - this is where we could place client-side or server-side scripts that we can use to hook into Git's different lifecycle events

info directory - contains the global excludes file

objects directory - this directory will store all of the commits we make

refs directory - this directory holds pointers to commits (basically the "branches" and "tags")

Remember, other than the "hooks" directory, you shouldn't mess with pretty much any of the 
content in here. The "hooks" directory can be used to hook into different parts or events of Git's 
workflow, but that's a more advanced topic that we won't be getting into in this course.
