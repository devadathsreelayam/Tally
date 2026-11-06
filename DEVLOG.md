**1. What does git add actually do? What is the staging area for?**
The command `git add` adds a particular file to the staging area of git's tracking. The staging area is an intermediate step before committing the version into the local repository. The staging area keeps track of the changes to the files from its creation or last commit. Once committed, that version becomes the next code version.


**2. What’s the difference between merge and rebase, and when would a team ban one of them?**
Git merge merges two branches together while preserving the history. Existing commits are preserved. Rebase does the same but alters the history from the point where the new branch started. It creates a clean linear history.


**3. Why should a virtual environment never be committed?**
A virtual environment holds the library files and compiled python files which includes thousands of text files. They contribute heavily to the repository size and make it complex. A simple requirement file can download and build same dependencies using a pip install command.
