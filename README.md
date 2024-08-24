# Gitproject
git branch my-new-branch      // create a new branch
git branch                      // show all list of branches
git checkout my-new-branch   // switch master branch to new branch
git branch                   // show all list of branches


Syntax: Create Git Tag for Commit
git tag <tag_name> <commit_sha>

git revert************************
git revert is the safest way to change history with Git. Instead of deleting existing Commits, git revert looks at the changes introduced in a specific Commit, and then applies the inverse of those changes in a new Commit. It functions as an "undo commit" command without sacrificing the integrity of your repository's history. git revert is always the recommended way to change history when it's possible.

You can use the command "git revert commitid" to rollback and revert specific Commits.


git reset**********************************
Sometimes, a Commit includes sensitive information and needs to be deleted. git reset is a very powerful command that may cause you to lose work. By resetting, you move the HEAD pointer and the branch pointer to another point in time - maybe making it seem like the Commits in between never happened! 
git reset --hard (commitid)  (Revert and rollback some existing Commits but cannot forward)

Before using git reset:
Be sure to talk with your team about any shared Commits.
Research the three types of resets to see which is right for you (--soft, --mixed, --hard).
Commit any work that you do not want to be lost intentionally — work that is committed can be retrieved; uncommitted work cannot be retrieved.

