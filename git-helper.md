
first of all HEAD is a pointer, out working things are always in a pointer named HEAD.
> we can change HEAD position using checkout
----------------------------------------------------------


showing all branch log--
>git log --all --oneline
----------------------------------------------------------
  
  
showing current branch log 
>git log --oneline
----------------------------------------------------------


rollback to any previous commit (no new commit will be executed, this for the time when we just need to go to a previous version and it wont
                                 matter if the commits after the given "commit_id" is deleted)
```
git reset <commit_id>
git push --force
```
----------------------------------------------------------



if we want to go to a previous version but we don't want to delete the commits that are committed after the given "commit_id" then
we should use revoke
a good tutorial link
>https://www.freecodecamp.org/news/git-revert-commit-how-to-undo-the-last-commit/
>https://stackoverflow.com/questions/4114095/how-do-i-revert-a-git-repository-to-a-previous-commit

```
git revert --no-commit <commit_id> -m 1(m is needed if there is a merge commit in between head and 
git --continue
```
----------------------------------------------------------


=> shows all the local branches and the local version of the corresponding remote branches
>git branch -av 
-----
=> pulls all the remote branch updated version to local origin/<branch_name> 
>git pull  
-----
=> merge current HEAD position with the given <branch_name>
>git merge origin/<branch_name> 
----------------------------------------------------------
----------------------------------------------------------
----------------------------------------------------------

removing a file
[remove file to reflect other branch](https://stackoverflow.com/questions/2047465/how-can-i-delete-a-file-from-a-git-repository/2047477)
----------------------------------------------------------
