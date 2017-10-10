# How did viewing a diff between two versions of a file help you see the bug
that was introduced?

Helps you pinpoint the exact location of the difference

# How could having easy access to the entire history of a file make you a more efficient programmer in the long term?

Can correct any mistakes you make
Can revert to old file if you can't solve the problem
Don't have to find issues manually

# What do you think are the pros and cons of manually choosing when to create a commit, like you do in Git, vs having versions automatically saved, like Google Docs does?

Con = if you have any issues i.e. your computer crashes, you may not be able to recover the latest version of your work

Pro = you can make commits which make coherent sense i.e. find a good breakpoint in your code

# Why do you think some version control systems, like Git, allow saving multiple files in one commit, while others, like Google Docs, treat each file separately?

Because some sets of files are relational i.e. they work as a group and changes in one will mean changes in another. Therefore in order to get a good picture of what changed you need to look at changes across the whole group

You wouldn't expect google docs files to be interdependent

# How can you use the commands git log and git diff to view the history of files?

Git log shows you all the past commits (most recent first). With Git diff you can compare two - if you want to see what changed in log ID x, compare it to the one below it (y): "git y x" (git <original> <new>)

# How might using version control make you more confident to make changes that could break something?

Because you know you could use git checkout to go back and find out where an issue was introduced and if needed revert to that version