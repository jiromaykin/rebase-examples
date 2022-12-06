# rebase-examples

Learning rebase and squash and stash.
Here I add a merge conflict.

git rebase -i main

the WIP commit is fine, I change pick into fixup, :wq and rebase is ‘done’

now push to the remote, with force, since we rewrote history:

git push --force-with-lease
