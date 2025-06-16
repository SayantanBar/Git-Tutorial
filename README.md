1. `git init` --> Power your folder to managed by git, and initialized a new empty repository. It also creates a .git folder that has all relevent logic to manage versions of your project.

2. `working area` --> There can be bunch of files that are not currently handle by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area, is consider to be not in the staging area. When we do `git status` and we see a bunch of `untracked files` then these are actually called to be in the working area.

3. `Staging area` -> What all files are going to be part of that next version that we will create. This staging area is the place what git knows what changes will be done from the last version to the next version.

4. `Repository area` -> This area actually contains the details of your previous registered version. And the files in the area, git already manages them and know their version history.

5. `git add <files>` -> moves the file from working area to staging area.

6. `git rm --cached <filename> ` -> moves file back from staging area to working area.

7. `Commit` -> Commit is the particular version of the project. It captures a snapshot of a project staged changes and creates a version out of it.

8. `git commit` -> Register a staging changes to a commit.

9. `git log` -> List down all the commits of the repository.

10. `git restore <filename>` -> It removes all file changes from staging area to be commited. This can be useful, If we did some dirty piece of code and now no more want it, Instead of deleting every changes line by line, we can `restore` it or you can say restore last clean version of the file.

11. `git restore --staged <filename>` --> It removes file from changes from staging area to working area.

12. Diff between git rm and git restore :

- Ans : If you want to move the whole file back to the untrack state, then we do `git rm`. Otherwise if we want the changes to be moved in working area or staging area then we do `git restore`

13. `git diff commit1 commit2` -> Gives the difference between all file changes between two commit.

14. `git remote` -> List down all the remote connection names.

15. Remote connection -> It helps you to link two git repositories for uploading and downloading changes from each otherwise

16. `git remote add <name of the origin> <link of the remote>` -> This command helps us to add a new link to the remote repo and give a new name to it.

17. `git remote rm <name of the remote>` -> This command deletes a remote conncection.

18. `git remote rename <old name><new name>` : This command renames the remote connection.

Note : The name of the remote conncetion is always used to establish communication between repos.
merge conflicts are very common scenario.

19 : `git add .` -> to add all files to staging area.

20 : `git pull <remote name> <branch name>` -> Download latest change from the branch of the mention remote in your local repo.
