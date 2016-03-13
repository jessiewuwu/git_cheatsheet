Git notes!
step one: make some changes
step two: `git add`
---
step three:
git reset
	to go back to last commit but your current changes are still here, just not staged
	* go back to last commit w/ current, unstaged changes

git reset --soft <commit>
	to go back to that specific commit, the changes will be unstaged. all the changes will be there  for example, the two files you changed are there, it's like you never did `git add`.
	* to go back to specific commit with unstaged changes 

git reset --hard HEAD^1
	to go back to last commit, throw away everything (you have no new changes to stage)

git reset --hard <commit>
	* to go back to specific commit and discard all changes

git checkout .
	(1) if you did `git add .` already, the changes are there but need to be commited
	(2) if you didn't, all the changes will disappear


	---
okay lets make some changes
wait are git reset --soft HEAD^1 and git reset the same? They both go back to the previous commit. yeah. 


see who changed what and when in <file>
$ git blame <file>

show changes over time for <file>
$ git log -p <file>

go back to last commit w/ current, unstaged changes
$ git reset

go back to <commit> with unstaged changes 
$ git reset --soft <commit>

go back to <commit> and say goodbye to all your changes
$ git reset --hard <commit>

if nothing works, walk away from the keyboard



