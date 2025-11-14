## Learning Guide for Git commands and Git Hub

# Create a Local Repository using git commands
1. Create a folder Local drive (eg: C:)
2. Initiate the default branch name as "main" by the following command
        git config --global init.defaultbranch main
3. Initiate the author for the repository by the following commands
        git config --global user.name "username" (If there is a space in username use doublequotes)
        git config --global user.email "useremail" (If there is a space in useremail use doublequotes)
4. Initiate the repository by the following command
        git init
        which results as "Initialized empty Git repository ....   as there is nothing to commit

# Create a Repository in GitHub
1. Loginto your GitHub Account
2. Create New Repository and assign to "Private" or "Public" as your preference

# Push Local Repository to remote
1. Navigate to "Code" tab of your Git/hub Repository and follow the instructions to push repository
2. In this case, using Gitbash
    git remote add origin "use the link from the GitHub page"
3. Ensure that the remote link is added in local by the below commands
    git remote show origin or git remote -v
    Note: The Head branch will be shown as unknow, since there is no commits have done yet

# First Commit and pushing to remote
1. Create a new file in the above mentioned folder/repository in Gitbash
    In this case, 
    touch instructions.md
2. Edit the file
    start instructions.md
3. Add the file into the repository for commiting
    git add instructions.md
4. Commit the file to update the changes  with message (user defined)
    git commit -m "First commit"
5. To know the status of the file or folder
    git staus - which results the status of the folder
6. Push the changes to remote
    git push -u origin main



### Creating New Brach to the Repository
1. Create new branch to the Repository
    In this case,
        git checkout -b branch_instructions
2. Add content into file (instructions.md) which will be under new branch
3. Push to the remote by the following command
    git push --set-upstream origin branch_instructions
    which allows you to push the file to remote from the new branch directly (you can merge this in GitHub)
    Ensure on GitHub you can able to see the Pull request page
4.  On GitHub "Create the Pull request"
5.  Once the Pull request updated, Confirm the "Merge Pull request"
6. Then switch to Main branch


    Note: git log --oneline command shows the information about the logs


### Testing for Assessment
1. Pushing changes to main and accessible in GitHub without PR
