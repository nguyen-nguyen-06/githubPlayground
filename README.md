# githubPlayground

This is where I start learning gitHub

This is the first subheader 
## Some useful things when using git

1) Have a repository: 
Follows: create a folder to work with, git clone, git add . (this is to tell git to keep track changes in all the directory), git commit -m "some message" (suggest change, usually need authors of the change git config user.name ot user.email), If I am the owner of the repository: git push (make change in the branch). 
2) Does not have a repository but have a folder
Follows: Create one, git init ( to create a .git file that keep track the change of the files), git add ., git commit -m "", git remote add origin \<URL of the repository\> (because commit is the update the change in local machine not on github. Since we have not connect the folder with any of the repository we have to add this line), git remote -v(to check the connection), git push


## Branching
create a new branch (git checkout -b \<branch name\>), (must in the new branch before) make some changes then save (git add ., git commit -m ""), (this changes will not appear on the other branch until we merge them).
Here we will have 2 choices.
1) if we believe our code is right or working independently(No need for review): (we should be in the branch that we want to be merged to) simply merge the new branch to the branch we want: 
git merge \<branch name\>
- Note: after we merge, this only change in local machine, we need to push to github 
2) If working with a team: after we commit, I need to push to github. Since I only create changes in local machine, I should create a new branch in github for those change by: 
git push -u origin \<branch name\> 
Then create a pull request ( a request to merge the branch to the branch we want)
If I am the owner, use: git pull (this will merge)


Then, after merging successfully, delete branch by git branch -d \<branch name\>

## Some useful things on terminal
1) When using bash in terminal, to check the bash profile(there are some code that I pasted to customize) use 
nano ~/.bashrc
2) When using powershell in terminal, to check the profile(there are some code that I pasted to customize) use
notepad $PROFILE
3) Some useful command in powershell + bash:
 - cd .. (Powershell)/ cd - (bash): this is to return to the closest parent of the the current directory
 - cd \<name\> (both) is to change the directory 
 - ls (both) is to see the child of the current directory
 - git status (both) is to see the status (keeptrack, commit) of the directory
 - git config user.name/ git config user.email : to see the name/email of the author of this commit 
 - git checkout -b \<name\>: to create a new branch
 - git checkout \<name\>: to change to a designated branch
 - clear: to clear the terminal screen
 - git commit -m "" -m "" : the first is header, the 2nd is message
 - git branch: to see the list of branch and the current branch we are in(this actually shown on the last word of the prompt, can modify this by accessing the profile)
 For the next 2 we should be in the branch we want to be merged to do that.
 - git merge \<branch name\>: to merge a specified branch with the branch we are in 
 - git diff \<branch name\>: show the total difference between the branch and the branch we are in



