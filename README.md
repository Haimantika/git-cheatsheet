GitHub is a Git repository hosting service, but it adds many of its own features. While Git is a command line tool, GitHub provides a Web-based graphical interface. It also provides access control and several collaboration features, such as a wikis and basic task management tools for every project.

# How to Install:

GitHub provides desktop clients that include a graphical user interface for the most common repository actions and an automatically updating command line edition of Git for advanced scenarios.

**GitHub for Windows:**
 https://windows.github.com
 
**GitHub for Mac :**
https://mac.github.com
Git distributions for Linux and POSIX systems are available on the official Git SCM web site.

**Git for All Platforms:**
 https://git-scm.com

---
A *repository* is usually used to organize a single project. Repositories can contain folders and files, images, videos, spreadsheets, and data sets – anything your project needs. We recommend including a README, or a file with information about your project. GitHub makes it easy to add one at the same time you create your new repository. It also offers other common options such as a license file.
**To create a repository:**
1.       In the upper right corner, next to your avatar or identicon, click  and then select New repository.
2.       Name your repository (any name of your choice).
3.       Write a short description.
4.       Select Initialize this repository with a README.
 

---
*Branching* is the way to work on different versions of a repository at one time.
By default your repository has one branch named master which is considered to be the definitive branch. We use branches to experiment and make edits before committing them to master.
When you create a branch off the master branch, you’re making a copy, or snapshot, of master as it was at that point in time. If someone else made changes to the master branch while you were working on your branch, you could pull in those updates.
 
**To create a new branch:**
1.       Go to your new repository (any name you want).
2.       Click the drop down at the top of the file list that says branch: master.
3.       Type a branch name, readme-edits, into the new branch text box.
4.       Select the blue Create branch box or hit “Enter” on your keyboard.

---

On GitHub, saved changes are called commits. Each commit has an associated commit message, which is a description explaining why a particular change was made. Commit messages capture the history of your changes, so other contributors can understand what you’ve done and why.
**How to commit changes:**
1.       Click the README.md file.
2.       Click the  pencil icon in the upper right corner of the file view to edit.
3.       In the editor, write a bit about yourself.
4.       Write a commit message that describes your changes.
5.       Click Commit changes button
 
 ---

Pull Requests are the heart of collaboration on GitHub. When you open a pull request, you’re proposing your changes and requesting that someone review and pull in your contribution and merge them into their branch. Pull requests show diffs, or differences, of the content from both branches. The changes, additions, and subtractions are shown in green and red.
**How to merge pull request:**
In this final step, it’s time to bring your changes together – merging your readme-edits branch into the master branch.
1.       Click the green Merge pull request button to merge the changes into master.
2.       Click Confirm merge.
3.       Go ahead and delete the branch, since its changes have been incorporated, with the Delete branch button in the purple box.
 
---
## SOME GO TO COMMANDS IN GITHUB AND THEIR USES:
 
### MAKE CHANGES
1.    $ git status
 <p> Lists all new or modified files to be commited.</p>
2.    $ git add [file]
<p> Snapshots the file in preparation for versioning $ git reset [file] Unstages the file, but preserve its contents. </p>
3.    $ git diff
 <p> Shows file differences not yet staged. </p>
4.    $ git diff --staged
<p> Shows file differences between staging and the last file version </p>
 5.   $ git commit -m "[descriptive message]"
<p> Records file snapshots permanently in version history </p>

####  CONFIGURE TOOLING
Configure user information for all local repositories
 1.    $ git config --global user.name "[name]"
<p> Sets the name you want atached to your commit transactions </p>
2.     $ git config --global user.email "[email address]"
<p> Sets the email you want atached to your commit transactions </p>
3.     $ git config --global color.ui auto
<p> Enables helpful colorization of command line output </p>

##### CREATE REPOSITORIES
 Start a new repository or obtain one from an existing URL
1. $ git init [project-name]
 <p> Creates a new local repository with the specified name </p>
 2.$ git clone [url]
<p> Downloads a project and its entire version history </p?
 
###### GROUP CHANGES
Name a series of commits and combine completed efforts
1. $ git branch
<p>  Lists all local branches in the current repository </p>
2. $ git branch [branch-name]
<p> Creates a new branch </p>
3. $ git checkout [branch-name]
 <p> Switches to the specified branch and updates the working directory </p>
 4.$ git merge [branch]
<p> Combines the specified branch’s history into the current branch </p>
 5.$ git branch -d [branch-name]
<p> Deletes the specified branch </p>

###### REFACTOR FILENAMES
 Relocate and remove versioned files
1. $ git rm [file]
 <p> Deletes the file from the working directory and stages the deletion </p>
2. $ git rm --cached [file]
<p> Removes the file from version control but preserves the file locally </p>
3. $ git mv [file-original] [file-renamed]
<p> Changes the file name and prepares it for commit </p>
 
#### REVIEW HISTORY
 Browse and inspect the evolution of project files
1. $ git log
<p> Lists version history for the current branch </p>
2. $ git log --follow [file]
<p> Lists version history for a file, including renames </p>
3. $ git diff [first-branch]...[second-branch]
<p> Shows content differences between two branches </p>
 4. $ git show [commit]
<p> Outputs metadata and content changes of the specified commit </p>

##### REDO COMMITS
Erase mistakes and craft replacement history
1. $ git reset [commit]
 <p> Undoes all commits afer [commit], preserving changes locally </p>
2.$ git reset --hard [commit]
<p> Discards all history and changes back to the specified commit </p>

###### SYNCHRONIZE CHANGES
Register a repository bookmark and exchange version history
1. $ git fetch [bookmark]
 <p> Downloads all history from the repository bookmark </p>
2. $ git merge [bookmark]/[branch]
<p> Combines bookmark’s branch into current local branch </p>
 3. $ git push [alias] [branch]
<p> Uploads all local branch commits to GitHub </p>
4. $ git pull
<p> Downloads bookmark history and incorporates changes </p>
 
#### SAVE FRAGMENTS
 Shelve and restore incomplete changes
1. $ git stash
<p> Temporarily stores all modified tracked files </p>
 2. $ git stash list
<p> Lists all stashed changesets </p>
3. $ git stash pop
 <p> Restores the most recently stashed files </p>
4. $ git stash drop
<p> Discards the most recently stashed changeset </p>
