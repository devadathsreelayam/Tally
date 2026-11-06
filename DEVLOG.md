### 07-11-2026 - Setup virtual environment, updated license, completed assignemnt 0

#### Assignemnt 0

**MIT Licnese**

- What is allowed: Commercialisation, modification, distribution, sublicensing, private use, selling
- What is not allowed: Removing notices, holding authors liable, using names for endorsement, delete the original licensse file.

**1. What does git add actually do? What is the staging area for?**
The command `git add` adds a particular file to the staging area of git's tracking. The staging area is an intermediate step before committing the version into the local repository. The staging area lets developers build deliberate commits. If five files were changed for two unrelated reasons, you can stage and commit them as two clean commits.

A file once stages but edited will appear as staged and unstaged because, it tracks changes and not files. The first one takes a snapshot of the file when you added to the staging area (staged). The second one takes the snapshot of the newly edited file. So both exist simultaneously as one single file.


**2. What’s the difference between merge and rebase, and when would a team ban one of them?**
- **Merge** creates a new commit with two parents, unless it can fast-forward. Look up what a fast-forward is.
- **Rebase** doesn’t “alter history from the point the branch started.” It replays your commits on top of a new base, creating brand-new commits with new hashes. The originals are abandoned.

A fast-forward merge in Git occurs when you merge one branch into another, and the target branch has not received any new commits since the source branch was created.


**3. Why should a virtual environment never be committed?**
A virtual environment holds the library files and compiled python files which includes thousands of text files. They contribute heavily to the repository size and make it complex. On top, the environment files are not portable because they contain absolute path to the local directory in which they were created on. A simple requirement file can download and build same dependencies using a pip install command.
