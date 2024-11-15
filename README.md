Hello, These are the steps I have followed to create this repository and performed actions such as Mergind, Rebasing, Deleting commits and retrieving, cherry-picking, reset, revert, etc,.


CLONING A REPOSITORY:

1. Went to the repository I wanted to clone and copied the Repository's HTTPS link.
2. Went to Folder where I want to clone this project through terminal.
3. Did => git clone <repository's https url>
4. New folder with project name was created and all the files of the project were cloned there.


MERGING TWO BRANCHES:

1.Created test1 and test2 branches individually from main branch.git checkout -b test1 and git checkout -b test2 on main branch.
2.Made changes in both the branches and committed. => git add . => git commit -m "message"
3.Went to main branch and merged both test1 and test2 branch, resolved merge conflicts manually and committed the changes.


REBASING MERGING AND RESOLVING CONFLICTS:

1.Created featureA and featureB branches form main branch.
2.Made changes in both the branches.
3.Rebases featureB onto featureA. => git rebase featureA
4.Now merged featureB and featureA on featureB branch.
5.Deleted featureB => git branch -D featureA.


CREATING A POST-COMMIT HOOK:

1. Navigated to hooks folder present in [.git] folder.
2. Created post-commit.txt file and added the following shell code.
#!/bin/bash

echo "I am a post commit hook"


CHERRY-PICKING:
1. created a c1 branch from main branch.
2. created a c2 branch from c1 branch.
3. Made necessary changes in c2 branch and committed.
4. On main branch I cherry picked the commit done by c2 branch. => git cherry-pick <commit-hash of c2>

