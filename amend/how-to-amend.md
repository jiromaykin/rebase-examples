# How to amend
## change commit messages after push

view your last commits (is used to display the output as one commit per line. It also shows the output in brief like the first seven characters of the commit SHA and the commit message):

$ `git log --oneline`

Now rewrite the git history with interactive rebasing of the last 5:

$ `git rebase -i HEAD~5`

You now need to specify the commits you wish to edit – by **picking** them:
