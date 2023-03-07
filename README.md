# Rebase-examples

Go here for [the 'amend'](amend/README.md) workflow.

Go here for [squashing lots of commits](squish/README.md) into 1 commit.

## When to Squash Your Commits

Combine multiple existing commits into a single one. Squashing commits is the preferred way to merge a feature branch back into a long-running branch like "main".

### using Git's "Interactive Rebase" feature

```$ git rebase -i HEAD~3```

If you mark one or more lines as "squash", they will be combined with the one above.

After entering a commit message for the new, combining commit, the Interactive Rebase is completed.

now push to the remote, with force, since we rewrote history:

```$ git push --force-with-lease```

---

### Merge conflicts

Learning rebase and squash and stash.
Here I add a merge conflict.

Let’s say a feature branch is started.
(git config --global pull.rebase)Let’s say a feature branch is started.
(git config --global pull.rebase)

git checkout main && git pull origin main

git rebase -i main

the WIP commit is fine, I change pick into fixup, :wq and rebase is ‘done’

git checkout main && git pull origin main
now push to the remote, with force, since we rewrote history:

git push --force-with-lease

squash commits before rebasing on develop.

now push to the remote, with force, since we rewrote history:

git push --force-with-lease

So many merge conflicts!
