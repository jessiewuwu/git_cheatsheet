Git notes!

git reset
	to go back to last commit but your current changes are still here, just not staged

git reset --soft HEAD^1
	to go back to last commit, the changes will be unstaged. for example, the two files you changed are there, it's like you never did the commit. 

git reset --hard HEAD^1
	to go back to last commit, throw away everything (all staged edits)

git checkout .
	(1) if you did `git add .` already, the changes are there but need to be commited
	(2) if you didn't, all the changes will disappear

	