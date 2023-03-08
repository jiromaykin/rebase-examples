# Squash 'n squish

Branches: main and feature/squish

First work in feature/squish and push + created Pull Request.

Then go to main: $ git checkout main && git pull origin main

Set rebasing correctly: $ git config --global pull.rebase true

Check-out your feature branch and ask for a rebase: $ git rebase -i main

In the VIM rebase file, type 'i' in order to insert fixup = like "squash", but discard this commit's log message. Hit 'Escape' and type :wq to save and exit.

You will probably be able to do a $ git rebase --continue from the usual terminal here, and after that get the $ git status to see your remote branch is diverging, which is good, then $ git push --force-with-lease and you should be all set and ready to merge,


1st line.

2nd line.

3rd line.

4th line.

Badly explained: https://www.maykinmedia.nl/blog/2017/nov/20/git-rebasing-make-your-commit-history-pretty/
