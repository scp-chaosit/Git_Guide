# Most Useful Git Commands
this is statement of most useful git commands (well, at least I think so; of course you can have a different opinion)

## `git init`:
> uses to initialize an empty git repo

## configure levels
> system (all users): `git config --system`<br>
> global (current user): `git config --global`<br>
> local (current repo): `git config --local`

## `git config --global core.editor "editor"`:
> makes git use the editor that was stayed in quotes in messages (like writing a commit)

## `git config --global user.name "name"`:
> makes git attach your name that was stood in quotes be attached to your commits

## `git config --global user.email "email"`:
> makes git attach your email that was stood in quotes be attached to your commits

## `git --unset`:
> allows you to unset something, like `git config --global --unset user.name`

## `git config --global init.defaultBranch <branch>`:
> will set your repos default branch (default branch: main)

## `git add <file>`:
> stages a file

## `git add -A`:
> stages all files

## `git restore --staged <file>`:
> unstages a file

## `git commit`:
> opens your default editor, letting you write a long message to your commit

## `git commit -m "message"`:
> commits staged changes with a following message

## `git commit -a -m "message"`:
> commits all tracked changes with a following message (skips stagging)

## `git log`:
> allows you to see commit history (logs)

## `git tag <tagname>`:
> creates a lightweight tag

## `git tag -a <tagname> -m "message"`:
> creates an annotated tag

## `git tag <tagname> <commit_hash>`:
> tag a specific commit (something like git tag v1.1 1234abcd : v1.1 - tag; 1234abcd - commit hash)

## `git tag`:
> lits tags

## `git show <tagname>`:
> shows tag details

## `git push <branch> (usually branch is origin - uses instead of a name for your remote repo) <tag>`:
> pushes a tag to defined branch in a repo<br>
> WARNING: if you'll just use `git push`, it WON'T push your tags!<br>
> you mush push tag explicity

## `git push --tags`:
> pushes all your local tags to a remote repo

## `git tag -d <tag>`:
> deletes a tag locally

## `git push <branch> --delete tag <tag>`:
> deletes a tag from remote repo

## `git tag -f v1.0 <new_commit_hash>; git push --force origin v1.0`:
> updates or replaces a tag (force push)

## `git stash`:
> stashes your changes

## `git stash -u`:
> stashes your changes (including untracked files)

## `git stash -m`:
> stashes your changes with a message

## `git stash list`:
> lists all stashes

## `git stash show`:
> allows you to see all changes from a previous stash

## `git stash branch <branch_name>`:
> creates a new branch from a stash

## `git stash apply`:
> restores your most recent stashed changes (keeps the stash in the stack)

## `git stash apply stash@{n}`:
> restores a specific stash (replace n in curly brackets to the number of your stash, like `git stash apply stash@{1}`)

## `git stash pop`:
> applies the latest stash and removes it from the stack

## `git stash drop stash@{n}`:
> "drops" (deletes) a specific stash when you no longer need it

## `git stash clear`:
> deletes all the stashes

## `git stash branch <branch_name> stash@{n}`:
> creates a new stash and applies your stashed changes<br>
> useful if your stashed work should become its own feature branch

## `git log`:
> show full commit history

## `git log --online`:
> show a summary of commits

## `git show <commit>`:
> show details of a specific commit

## `git diff`:
> show unstaged changes

## `git diff --staged`:
> show staged changes

## `git diff <commit1> <commit2>`:
> compares two commits
