# __GIT AND GITHUB__

## Terminal basics
opening the pwd using the commandline/terminal
for windows:
```bash
start .
```
for linux:
```bash
open .
```
the . means the cwd. You can open any folder that is in that pwd in the file explore.

### other important commands
1. cd - change directory

1. ls - list items in a folder
1. touch - creating a file
1. mdir - creating a folder
1. rm & (rm -rf) - to remove a file and folder respectively

## what is a repo
a workspace which tracks and manages files within a folder.

### how to start a repo
in your pwd, open the terminal and run the command:
```bash
git init
```
it creates a hidden folder .git that tracks all the changes and keeps the history.
__Note__: if you delete the .git folder the repo will cease to exist

### git status
gives information on the current status of a git repository and its contents.

### working area
this is where you will create your files and folders, edit and delete them (it is the repo)

### git add thefile/--all/ .
puts the changes in the staging area ready to be committed

### staging area
this is where changes are assembled when the git add command is used. You can add files that you want and ignore those that you dont want. It shows the created files, modified files and deleted files.

### git commit -m / -am "message
it is used to save changes in your local repository.
-m means set the commit message (MANADATORY)
-a means including all currently changed files in the commit (optional)

### git log
displays all of the commits in a repository's history
