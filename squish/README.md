# Squash 'n squish

Branches: **main** and **feature/squish**

First work in _feature/squish_ and push + created _Pull Request_.

Then go to main: $ `git checkout main && git pull origin main`

Set rebasing correctly: $ `git config --global pull.rebase true`

Check-out your feature branch and ask for a rebase: $ `git rebase -i main`

In the VIM rebase file, type '`i`' in order to insert `fixup` = like "squash", but discard this commit's log message. Only '`pick`' your oldest/first commit - and 'fixup' all the others, bu do a '`fixup -C`' in order to keep the text of your last commit message, if that is the text you want o keep. Hit 'Escape' and type :wq to save and exit.

`pick [1] Ugly commit message`

`fixup [2] Ugly commit message`

`fixup [3] Ugly commit message`

`fixup -C [4] Clear good message`

This results in just 1 commit with the Clear good text.

You will probably be able to do a $ `git rebase --continue` from the usual terminal here, and after that get the $ `git status` to see your remote branch is diverging, which is good, then $ `git push --force-with-lease` and you should be all set and ready to merge.

Or use the GUI of Github:

https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/managing-commits/squashing-commits

Badly explained: https://www.maykinmedia.nl/blog/2017/nov/20/git-rebasing-make-your-commit-history-pretty/
