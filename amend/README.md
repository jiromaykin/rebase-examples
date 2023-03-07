# How to amend
## change commit messages after push

view your last commits (is used to display the output as one commit per line. It also shows the output in brief like the first seven characters of the commit SHA and the commit message):

$ `git log --oneline`

Now rewrite the git history with interactive rebasing of the last 5:

$ `git rebase -i HEAD~5`

You now need to specify the commits you wish to edit – by **picking** them:

$ `e` = edit files; $ `r` = reword

Git will now step through each of the commits you specified and ask you to make your changes,

You can amend the commit now, with

        git commit --amend

Once you are satisfied with your changes, run

        git rebase --continue

If you do a git rebase -i without specifying a revision range you get all your unpushed commits, which is probably what you want to rebase anyways.

To quit the process:

$ `git rebase --quit`
