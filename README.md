git-toolbox
===========

A toolbox of convenient git tools.

git-clone-branches is a shell script for cloning only a specific set of branches
from a repository. In reality, it is really a wrapper around a "git init"
followed by "git remote add", but I find it handy whenever I want to get only a
specific branch or two from a repository.

git-empty-branch is a shell script for creating a branch in a repostory with no
history. This branch effectively has the state of the first, uncommitted branch
after a call to "git init". This is convenient if you want to start a branch
that has independent history from your other branches. For example, after
creating a bunch of coding branches, if you want to start a separate, fresh
branch for documentation, but you do not want a separate repository, this might
be handy.

git-ignore-from-svn:ignore is useful if you want to convert a Subversion repo's
svn:ignore properties into a .gitignore file (and you're not using git-svn).
You might want this if, for example,you checkout a svn repo and want to just
stick the code into a git repo.
