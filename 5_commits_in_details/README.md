# Commits in details

## keeping the commits atomic
means to try and keep each commit focused on a single thing example: a single feature, change or fix.
It makes it easier to undo or rollback changes later on. It also makes your project easier to review

for instance, you can create a folder and add images that will be used in your project. At the same time you can rename function name that is used in all files meaning modifying all the files that uses that function. When committing, it will be atomic if u commit twice:
1. 1st commit - add folder with images.
1. 2nd commit - renamed a certail function.

## configuring editors for git
u can use the command "git commit" without the message and this will prompt the system to open an editor. to configure your prefered editor:
1. for nano:
```bash
git config  --global core.editor "nano -w"
```
1. for vscode:
```bash
git config  --global core.editor "code --wait"
```

## Amending a commit
Helps to redo the previous commit (one commit ago)
you can do this if you have forgotten to commit a file or you want to edit the commit message.

for you to add the forgotten file/folder, you have to  add and stage it(ready to be commited) first b4 using the ammend command.
```bash
git commit --amend
```
it will prompt the default editor and edit the commit, if you have added a file it will also be included in that commit.

## the .gitignore file
it ignores files and folders which the user specifies. some of the files and folders that can be ignored are:
1. secret API keys, credentials etc
1. operating system files
1. log files from things like IDEs, programming languages etc.
1. Dependencies and packages

### ignoring files
1. __ignoring specific files__ 
just write the name of the file eg: todo.txt -this will ignore the file that is called todo.txt.
1. __ignoring folders__
use the forward slash at the end of the folder name (or just write the folder name) eg: folderName/ - this will ignore the folder and everything inside it.
1. __using wildcard characters(*)__  eg: *.log - will ignore all the files that start has the extension .log.
