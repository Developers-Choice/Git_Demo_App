1. `git int` -> Powers your folder to be managed by git, and initializes a new empty repository
repository. It also creates a .git folder that has all the relavant logic to managed
versions of your project.


2. `Working Area` -> There can be a bunch of files that are not currently handled by git.
It means that changes done or to be done in those files are not managed
git yet a file which is in working area is considered to be not in the staging area.
When we do `git status` and we see bunch of `untracked files` then these are actually called to be in the working area.


3. `Staging area` -> What all files are going to part of the next version we will create.
This staging area is the place where git knows what changes will be done from the
last version to the next version


4. `Repository Area` -> This area actually contains the details of all your previous registered version.
And the files in this area, git already manages them and knows there verison history



5. `git add <file>` -> moves file from working area to staging area


6. `git rm --cached <file>` -> moves file back from staging area to working area


7. `commit` -> Commit is a particular version of the project. It captures a snapshot of the project's staged
changes and creates a version out of it


8. `git commit` --> registers staging changes to a commit.


9. `git log` --> list downs all the commits of the repository. If you want to exit out of git log prompt
press `q`.


10. `git restore <files> ` --> it removes all files changes from the staging area to be commited.
this can be useful if we did some dirty peice of code now no want it. Instead of deleting every change line by line we can restore it
or we can say restore last clean version of the file.


11. `git restore --staged <file>` -> it removes file changes from staging area to the working area.
this only works if changes are in your staging area.

12. Diff between git rm and git restore
ans: if you want to move the whole file back to the untracked state, then we do git rm,
otherwise if we just want the changes to be moved in working area or staging are then we do git restore

13. `git diff commit1 commit2` --> gives the difference of allfile changes between two commits

14. `git commit -m "<your commit message>"` -> if we want to avoid opening a text editor like vim/nano to add commit message we can use 
this following command  


15. `git remote` --> list down all the remote connection names


16. Remote Connection --> It helps you to link two git repositories for uploading and downloading changes
from each otherwise


17. `git remote add <name of remote> <link of the remote>` : this command helps us to add a new link to the remote and give a name to it.



18. `git remote rm <name of remote>` : this command deletes a remote connection.


19. `git remote rename <oldname> <newname>` : this command renames the remote connection


Note: The name of the remote connection is always used to establish communication between the repos


20. `git add <file1> <file2> <file3>`: this command will add multiple file changes together in the staging area


21. `git add .`: this command will add all files from working repo to staging area.


22. Recommended Practice `git pull <remote name> <branch> ` : downloads latest changes from the branch of the mention remote in your local repo
    condition for pull: Your Working Dir should be clean, Your Staging Directory should be clean


### Recommended practice to do


     - make changes
     - git add <file>
     - git commit
     - git pull (developer's morning routine when they start open source 😂)
     - git push (remote name) (branch name)



Local Repo & Github Repo

For globally or teams accessible way we can achevie we 
connect Local Repo == Github Repo
using remote origin

rempo is modified

git remote add <-- your starting to connect with something 
writing origin is not neccessary Instead you can write
raafay and whatever name you like

Origin == Name of Remote Connection

Using Origin we will do operations cause origin refer's to.
the remote connection url from which we are connected to the github-repo which is on server


`stikcy note`
using add we will be moving from my working area where i made the homefresh changes lol
to stanging area which are now be considered as tracked files ready to be commited.
