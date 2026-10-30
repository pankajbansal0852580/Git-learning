# Git-learning
Git is a Version Control Tool
I am learning git from Edureka 
This is the URL of the yt video containing git and all about DevOps
https://www.youtube.com/watch?v=hQcFE0RD0cQ&t=3654s

# Step 0: Prerequisites
  Installed Git on system

# Step 1: Create Repo
  Made a folder for my local git repo in my D drive
  Right clicked and git bashed there
  Initialized empty repository by "git init" command

# Step 2: Syncing local and remote Repos
  Added remote repository as origin by "git remote add origin <link_of_remote_repo>" command
  Pulled the files from remote repo using "git pull origin main" command

# Step 3: Making changes
  Index is the layer between local project folder and local repo
  Need to add files to the index before committing them to repo
  Used "git status" to see files currently in the index
  Used "git add <file-name>" to add file to index (use -A flag to add all files at once)
  Used "git commit -m "commit message"" to commit changes to local repo(use -a flag to commit all files at once and also to explicitly commit tracked files without using git add)
  Used "git log" command to see the all the previous commits information

# Step 4: Parallel processing through branches
  A branch is a lightweight, moveable pointer to a specific commit.
  Used "git branch <branch-name>" to make a different branch 
  Used "git checkout <branch-name>" to navigate to that branch 
  Made a file in that branch, added and committed it 
  Moved to main branch, and saw that the local folder now doesn't show those files, since they are in another branch 
  Used "git merge <branch-name>" inside main branch to merge the other branch into it and now those files show up again in the local folder

# Step 5: Pushing to remote repository
  Created ssh key by "ssh-keygen -t ed25519 -C <email-address>" command
  Uploaded that public key to github
  Added private key by "ssh-add ~/.ssh/id_ed25519" command
  Authenticated to github using "ssh -T git@github.com" command
  Pushed first branch to central repo using "git push origin firstbranch" command, This makes a new branch on the central repo as well
  To push the main branch, Did this
  1. git pull origin main --allow-unrelated-histories
  2. ESC Then :wq then ENTER
  3. git push origin main 
  
# Step 6: Reverting back
  To revert back to a previous commit
  Copied its commit hash from the git log details
  Used the "git checkout <commit-hash> <file-name>" command to go back to the previous version of the file
  But this doesn't actaully commit that file to the index, it will still upload the updated version of the original file not the original reverted one
  To push that updated reverted version, do a git commit before it

AND THAT'S IT!! CONGRATS ON LEARNNG TO USE GIT!
