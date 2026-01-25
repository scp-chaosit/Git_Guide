# Most Useful Git Commands
this is statement of most useful git commands (well, at least I think so; of course you can have a different opinion)

## `git init`:
    uses to initialize an empty git repo
    
## configure levels:
    system (all users): `git config --system`
    global (current user): `git config --global`
    local (current repo): `git config --local`

## `git config --global core.editor "editor"`:
    makes git use the editor that was stayed in quotes in messages (like writing a commit)

## `git config --global user.name "name"`:
    makes git attach your name that was stood in quotes be attached to your commits

## `git config --global user.email "email"`:
    makes git attach your email that was stood in quotes be attached to your commits

## `git --unset`:
    allows you to unset something, like `git config --global --unset user.name`

## `git config --global init.defaultBranch <branch>`:
    will set your repos default branch (default branch: main)
