# Git-learning
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
  Used "git commit -m "commit message"" to commit changes to local repo(use -a flag to commit all files at once)
  Used "git log" command to see the all the previous commits information

# Parallel processing through branches
  A branch is a lightweight, moveable pointer to a specific commit.\n
  Used "git branch <branch-name>" to make a different branch \n
  Used "git checkout <branch-name>" to navigate to that branch \n
  Made a file in that branch, added and committed it \n
  Moved to main branch, and saw that the local folder now doesn't show those files, since they are in another branch \n
  Used "git merge <branch-name>" inside main branch to merge the other branch into it and now those files show up again in the local folder
  
  
