	1. Git (local)


init
git init

add
git add .

commit
git commit -m "add file"

check commit
git log

jump back to old commit (remove newer commits)
git reset --hard [git id]   (move HEAD to this git id, newer git will be no longer available)
*don't just use git checkout [git id], this will move this commit out of the branch

back to latest commit (move HEAD to the newest commit)
git checkout -- .

check branches
git branch

create new branch
git checkout -b new-feature (create a branch named new-feature)

navgate to branch
git master (goes to the master branch)

create new branch based on current branch
git checkout -b new-feature (create a branch named new-feature)

merge new branch to the master branch
	1) git master (goes to master branch)
	2) git merge new-feature (merge new-feature branch to the master branch)

merge branches with conflict contents
	1) git master (goes to master branch)
	2) git merge new-feature
	3) (select the content you want to accept, then delete comments in the file)
	4) git add .
	5) git commit -m "merge conflict resolved"

delete branch
git branch -D new-feature (delete new-feature branch)


GitHub (remote)
