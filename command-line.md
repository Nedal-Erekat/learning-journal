
# GIT INTRO:
#### Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes. Through version control, one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes.

#### Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.
##### Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data.
* Files in Git can reside in three main states: committed, modified and staged.
1.  Committed
Data is securely stored in a local database
 2.  Modified
File has been changed but not committed to the databas
3. Staged
Flagged a file’s changed version to be committed in the next snapshot

> $ cd test (cd = change directory)

### Cloning
#### You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

> $ git clone https://github.com/test
##### To clone a repository into a directory with another name of your choosing, use the following command format:

>$ git clone https://github.com/test mydirectory
##### The command above makes a copy of the target repository in a directory named “mydirectory.”
##### for cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch
#### To determine the state of files, utilize the git status command.

* Tracking and Staging a New File
   - Single File
      - Track one file only by using the following format:git add filename
   - All Files
     - Track all files in a repository by using the following command:

> $ git add . 

#### After staging one or multiple files, you should commit the changes and record what you did within the commit message:

> $ git commit -m “made change x,y,z”
--------------
### Committing All Changes
> $ git commit -a
* This command commits a snapshot of all modifications to tracked files in the working directory.
----------
## Pushing Changes
##### Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

* Example:

>$ git push origin master