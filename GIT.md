A git version control tool
it is a command line tool to keep track of changes to code as snapshots
Synchronizes code between different people using push and pull
Test changes to code without losing the original using branch and merge
Revert back to old versions of code
GIT is local whereas github is used to host this git content in repos
Work on GIT using command line whereas Github using web 

# GITHUB

holds files on a website called github using repositories

git init : intialises the .git folder to hold log content


git clone : takes a rep from internet to your local machine
                 git clone <url>

git add <filename> : it prepares the file or changes to be commited

git commit -m " " : takes snapshots whatever is prepared by add in the local system

git push : pushes the changes into the github

git commit -am " " :  all files gets add and commit
every commit produces a hash code (unique).

git works on adding and removing line , if two work on modifying a same line merge conflict might occur

git log : tell us the commit, author and id

git status : The git status command displays the state of the working directory and the staging area

git reset --hard <commithash>
git reset --hard origin/master

branches, head

git branch : tells us all the branches that exist and   (*) the branch the head points to

git checkout -b <branchname>

-b is only used for new branch 

git merge <branch_name>

FORKING
fork creates a completely independent copy of git repository.
clone creates a linked copy that will continue to synchronize with the target repo


git stash : not comitted but need those for later

git stash pop : bring back for work

git stash clear : clear

git remote add origin <link>

git push origin master

squash
git rebase -i <commit_id>



 
