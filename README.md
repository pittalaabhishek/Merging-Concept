Hello, These are the steps I have followed to create this repository and performed actions such as Mergind, Rebasing, Deleting commits and retrieving, cherry-picking, reset, revert, etc,.

For Merging two branches:
1.Created test1 and test2 branches individually from main branch.git checkout -b test1 and git checkout -b test2 on main branch.
2.Made changes in both the branches and committed. => git add . => git commit -m "message"
3.Went to main branch and merged both test1 and test2 branch, resolved merge conflicts manually and committed the changes.

For Rebasing Merging and resolving conflicts:
1.Created featureA and featureB branches form main branch.
2.Made changes in both the branches.
3.Rebases featureB onto featureA. => git rebase featureA
4.Now merged featureB and featureA on featureB branch.
5.Deleted featureB => git branch -D featureA.