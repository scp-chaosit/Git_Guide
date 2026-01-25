# what is git?
> git is a popular version control system that was created by Linus Torvalds in 2005<br>
> it is used for:
> - tracking code changes
> - tracking who made changes
> - coding collaboration

# key git concepts?
> - repository: a folder where git tracks your project and its history
> - clone: make a copy of a remote repository on your computer
> - stage: tell git which changes you want to save next
> - commit: save a snapshot of your staged changes
> - branch: work on different versions or features at the same time
> - merge: combine changes from different branches
> - pull: get the latest changes from a remote repository
> - push: send your changes to a remote repository

# what is staging environment in git?
> the staging environment (or staging area) is an environment (or an area) where you can "place" your changes (meaning files or directories) for the next work with them<br>
> this gives you control over what goes into your projects history (like if you want to show all your files/directories/features now or later)

# so I know what is staging environment... but what is staging exactly?
> well, staging is some sort of a proccess when you select something you want to work with into a staging area

# what is a commit?
> for yourself, you can imagine commits like saves in vidoe games: when you think you need to save your job, you are using commits (or stashes, will describe them a little bit later)<br>
> it records a snapshot of your files at a certain time, with a message describing what changed<br>
> and, because commits are some sort of saves, you can always go back to a previous commit if you need to<br>
> also, it is a good practice to use `git commit -m "message"` for short messages, and `git commit` for long messages: this will invoke a text editor that you setted up in `git config --global core.editor "editor"`<br>
> and, once again, it is a good practice to keep your commits:
> - short (50 characters or less) to increase readability
> - use the imperative mode (e.g., "Add feature", not "Added feature")
> - if your commit is long, leave a blank line after the summary, then add more details if needed
> - describe *why* the change was made, not just what changes
