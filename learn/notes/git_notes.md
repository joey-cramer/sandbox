Making PR and merging to develop.

Use the same instructions for merging to main.

1. Fetch remote changes: 
	- git checkout develop (switch to develop branch)
	- git pull            (copy changes from Stash)

2. Verify you are on the correct branch
	- git branch

3. Update your branch to include those changes, which you just pulled
	- git checkout <mybranch>
	- git rebase develop --> if complains about "Conflicts" --> ping for help :)

4. Copy/replace your new files.  (note that this is a good and safe method while new to Git, next step is to work on the files in your branch directly)

5. Run "git diff" to check the changes are as expected.

6. Tell git to take note of what you've changed
	- git add file1 file2 file3

7. git commit -m "SESDK-xyz + descriptive comment"


8. CHECKS:

- What did I change last?
	- git show
- Show me the history, who changed what
	- git log
- Where am I, do I need to do something?
	- git status
- Show me what I have changed with respect to develop (i.e., all my changes)
	- git diff develop


9. I'm ready to send my contribution
- git push (or 'git push -f' if needed)


10. Review comments received
	- Make needed changes locally
	- git add changed_file1 changed_file2
	- git commit -m "SESDK-xyz + descriptive comment"
	- git push -f

11. Reviewers happy, PR approved
	- git rebase -i develop. Remember to squash commits.
	- Repeat steps 1-3. (to bring changes, if someone has updated develop while receiving review comments or working locally)
	- git push -f
	- merge from Stash with button




For when pushing an empty commit
git commit --amend --no-edit

git push origin <your_branch> --force-with-lease


Unwanted but still valid method
git commit --allow-empty -m "Trigger Build"
-------

Pushing commit // Short version

#Ensure that you're on right branch
git status

#if not on right branch
git checkout Vincjo/XXXXX-xxxxx/UpgradeToRobotFramework6.0

#get all of the latest updates + branch infos
git fetch


#when wanting to clear everything in branch down to the bare commit, also you must choose which commit you start from
#will remove all commits after that commit id.
git reset --hard <commitid> 



# refreshes the branch and looks for things that may have happened elsewhere
$ git fetch

-----
1. Remove the Log lines
2. git add <file>
3. git commit --amend --no-edit
4. git push origin <branch> --force
5. PR auto-update and PR job should be triggered
6. PR approved
7. Use [Merge] to merge your branch to 'develop' 


1. Create new branch from 'main' (BitBucket)
2. Check out main branch locally (git checkout main)
3. Update your local main branch (git fetch), ALWAYS "git status" after git fetch, as I may need to do a "git pull".
4. Check out your new branch (git checkout <urbranch>)
5. Cherry pick commits from develop: git cherry-pick <commit hash 1> <commit hash 2>
6. Push the changes (git push origin <urbranch> --force)
7. Create new PR  (BitBucket)PR reviewed and approved (BitBucket)
8. Merge your branch to 'main' (BitBucket)
9. Delete your branch (BitBucket)
10. You're done : )