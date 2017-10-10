## When would you want to use a remote repository rather than keeping all your work local?

When you want to share code with the rest of your team. When you want to ensure that you have more than one copy, i.e. a backup in case of loss or damage to your computer. When you want to be able to work remotely on multiple machines. When you want to make your code public / open source / collaborate.


## Why might you want to always pull changes manually rather than having Git automatically stay up-to-date with your remote repository?

Because pulling files down might overwrite the work you have done on your local machine.

 
## Describe the differences between forks, clones, and branches. When would you use one instead of another?

* A fork is a clone of a repo that takes place on githubs servers. It also has the benefit of linking back to the original repo. You would do this when you want to make changes to someone else's repo, but you don't have permission / want to alter it directly. In this case you could clone the repo down ot your computer, make some changes and either host them yourself or suggest them back to the owner.
* A clone is a copy of a directory that also includes all of git's tracking info contained in the hidden .git folder. You would use it to copy a remote directory down to your local machine (or you could also clone a repo on your local machine but this is less common).
* A branch is a way to label commits so that you can access them without having to note down the commit ID everytime. This allows you to make changes that don't affect your production quality code, and then later merge them into the main branch. It also means you can have multiple streams being worked on at the same time.


## What is the benefit of having a copy of the last known state of the remote stored locally?
 
So that you can keep track of what has changed between the remote and local versions since your last sync and also choose when/whether/how to merge the remote branch into your own 
 


## How would you collaborate without using Git or GitHub? What would be easier, and what would be harder?

Without Git you would have to either make changes in a linear fashion, passing your codebase from one author to the next. Or work simultaeneously and track changes / identify diffs/conflicts in some other way. Without Github it would be harder to share your code with a community, harder to suggest changes to someone else's codebase, harder to access your code remotely, and harder to have someone OK your work before incorporating the changes into the team's shared code.


## When would you want to make changes in a separate branch rather than directly in master? What benefits does each approach have?

Making changes directly into the master has the advantage that it is less of a faff - you don't have to deal with merging & resolving conflicts etc. You would use branches so that you can keep a 'ready to ship' copy of your code (the master branch) and also at the same time add new features or make experimental changes, which are clearly labelled as such. You can also use a branch to create a pull request, which allows you to get feedback on your code before you update master.


