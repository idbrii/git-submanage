git-submanage
=============

Simple scripts to manage git submodules


## git-sub-commit-changelog
Commit the changelog for a pending submodule

Commits the updated submodule with the changelog as the commit description.


## git-sub-ff-and-commit
Grab master if it's at our current commit, skip to origin's master, commit a
changelog to parent repo.

To apply to all submodules, you can use:

    git submodule foreach "cd - ; echo git sub-ff-and-commit \$name $*"


## git-subupdate
Apply remote changes to submodules.

Sync all urls, update HEAD to match remote, and use master branch if it's at
HEAD.


## git-use-branch-if-already-there
Checkout input branch if it matches the current commit

Useful to ensure submodules are using a branch (since they're usually at the
same commit as master, but the branch isn't automatically checked out).
