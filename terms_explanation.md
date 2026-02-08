# what is git?
> git is a popular version control system that was created by Linus Torvalds in 2005<br>
> it is used for:
> - tracking code changes;
> - tracking who made changes;
> - coding collaboration

# key git concepts:
> - *repository*: a directory where git tracks your project and its history;
> - *clone*: make a copy of a remote repository on your computer;
> - *stage*: tell git which changes you want to save next;
> - *commit*: save a snapshot of your staged changes;
> - *branch*: work on different versions or features at the same time;
> - *merge*: combine changes from different branches;
> - *pull*: get the latest changes from a remote repository;
> - *push*: send your changes to a remote repository

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
> - short (50 characters or less) to increase readability;
> - use the imperative mode (e.g., "Add feature", not "Added feature");
> - if your commit is long, leave a blank line after the summary, then add more details if needed;
> - describe *why* the change was made, not just what changes

# what is a tag?
> for yourself, you can imagine tags like a bookmark or a label for a specific commit<br>
> tags are most often used to mark important points in your project history, like releases (`v1.0`, `v1.5.5`, etc)<br>
> tags are simple and reliable way to keep track of versions and share them with your team or users<br>
> some common tag types:
> - *releases*: tags let you mark when your project is ready for release, so you (and others) can always find that exact version later;
> - *milestones*: use tags to highlight major milestones, like when a big feature is finished or a bug is fixed;
> - *deployment*: many deployment tools use tags to know which version of your code to deploy;
> - *hotfixes*: if you need to fix an old version, tags make it easy to check out and patch the right code

# what is the difference between lightweight and annotated tag?
lightweight tag:
> just a simple name for a commit (no extra info, like an actual bookmark)

annotated tag:
> stores author, date and a message

# what are stashes in git? why use them?
> stashes let's you quickly save your uncommitted changes (if you need to fix bug or something else) and return to a clean working directory<br>
> common use cases:
> - *switch branches safely*: save your work before changing branches;
> - *handle emergencies*: stash your work to fix something urgent, then restore it;
> - *keep your work-in-progress safe*: avoid messy commits or losing changes;

# what gets stashed if I'll use `git stash` or `git stash -u`?
> if you type `git stash`, this will stash all your tracked files<br>
> if you type `git stash -u`, this will stash both your tracked and untracked files

# what is difference between tracked and stashed files?
> tracked files in git are files that git is aware about: you used them in previous commit (`git commit`)<br>
> stashed files in git are tracked files that have been marked for inclusion in the next commit (`git add`)

# some stash "best practices"?
> to make your stashes clear and understandable, you need to follow some rules:
> - *use clear messages when stashing*: `git stash push -m "message"`
> - don't use stashes as long-term storage—commit your work when possible
> - check your stash list regularly and clean up old stashes you no longer need

# this may sound silly... but why do I need history in git?
> well, this question really sounds stupidly, but it's also ok<br>
> git history is useful for tracking who and when made this change, so if something broke, you can find a working version<br>
> some good practices:
> - make frequent, meaningful commits to keep your history clear
> - write clear commit messages so you and your team can understand changes later
> - use `git log --oneline` for a quick overview of your commit history
> - use `git diff` before committing to review your work

# how do I veiw an author in history?
> use `git log --author="Author"`

# how do I see commits that were made some time ago?
> use `git log --since="2 weeks ago"`<br>
> and, if you want to see a simple ASCII graph of your branch history, use `git log --graph` (it looks pretty good, idk what more can I say)
