# rebase-examples

Learning rebase and squash and stash.
Here I add a merge conflict.
Let’s say a feature branch is started.
(git config --global pull.rebase)

git rebase -i main

the WIP commit is fine, I change pick into fixup, :wq and rebase is ‘done’

git checkout main && git pull origin main