# What happens when you initialize a repository? Why do you need to do it?

A .git hidden directory is created which will contain all the tracking metadata associated with the repo

# How is the staging area different from the working directory and the repository? What value do you think it offers?

You can add files to the staging area before committing them; intermediate between the working directory and the repository. This allows you to choose which files you want to add. Can add multiple, one at a time, and then commit whole staging area bundled together

# How can you use the staging area to make sure you have one commit per logical change?

You can add files individually, use git diff to check they represent a logical change, and only then commit them. Can split files into smaller parcels

# What are some situations when branches would be helpful in keeping your history organized? How would branches help?

When you want to create a seperate version of a project but either you may wish to merge it back to the master later or you may wish to switch between the two (e.g. different language versions). Branches help as they allow you to label the different versions of your code so you easily know which one you are commiting to. Master branch = production quality code, ready to ship. Branches = new features, development work; think of it as context switching

# How do the diagrams help you visualize the branch structure?

It helps to see the flow backwards from child to parent, and to see at what points branches branched off or merged back in
 
# What is the result of merging two branches together? Why do we represent it in the diagram the way we do?

That the two separate code bases become one. Whichever branch you have checked out at the time becomes the head, so you say you merge branch b “into” branch a. The resulting commit then has two parents so you can access the commits from both branches from this one commit. When you run git log these are interleaved, ordered by timestamp. The label for the old merged branch (branch b) becomes redundant so you can delete it - you only need the label branch a to access all commits
 
# What are the pros and cons of Git’s automatic merging vs. always doing merges manually?

Main pro of automatic merging is convenience - save you the time of looking through every file. On the other hand you don’t want git to make the wrong decisions and include code which will break your program, therefore benefit of manually merging is that you have control over which code makes the final cut
