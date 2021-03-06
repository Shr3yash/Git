<div align="center">
  <p align="center">
  <img src="https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png?raw=true "Git"" width="350" title=🐱‍👤">
  
</p>

</div>

```sh
git --version
git config --global user.name
git config --global user.email
```
Create or Goto a directory
```sh
cd nameofdirectory 
```
or 
```sh
mkdir yourname   
```
initializes git staging environment in the directory blah(creates .git folder)
``sh
git init  
```
lists all added files in the directory
```sh
git ls  
```
gives insight of the content present in the directory
```sh
git status 
```
Staging:
Staged files are files that are ready to be committed , staging is just like asembling everything together.
Add files

```sh
git add filename
git add --all
git add-A
```
Until now was the staging part, now let's move on to commit.
Commit allows us to have a checkpoint on a specific status or version of the project files.
```sh
git commit -m "An eyecatching display message"
```
in this statement we committed all the sstaged files with a display message. We should include the message,
as it's a good practice to easily read the status through the commit message
Now, checking the status of our repository

```sh
git status --short
```
short is used above because it gives more insight on the status of our files as it appends(front) flags which denote:
?? - Untracked files
A - Files added to stage
M - Modified files
D - Deleted files

now, let's look into the log, to view the history of all the commits that is.
```sh
git log
```
to update the files with new version message :
```sh
git commit -a -m "Updated filename with a version"
```
All this stuff can also be learnt from git itself using this
```sh
git command -help
git commit -help
git help --all
```
just replace the command word with any command you want help with.
To list all possible commands, use the help --all command.

Branch: It is a seperate version of main repository. To create one such branch 
```sh
git branch branchname
git branch 
  branchname
* master
```
* denotes the current branch we are in. 
to change the branch

```sh
git checkout branchname
```
```sh
git checkout -b emergency-fix
Switched to a new branch 'emergency-fix'
```
 created a new branch from master, and changed to it. We can safely fix the error without disturbing the other branches. To fix bugs in master wtihout messing master directly and creating the clone then messing with it.
 
 ```sh
 git merge emergency-fix
 git branch -d emergency-fix
 Deleted branch emergency-fix (was dfa79db).
 ```
 merging the branch then deleting it.
 
 Conflicts :
 when there are differences between the file version in the common files of two branches that are to be merged, the merge conflicts occur
 ```sh
 ```
                    
                 
