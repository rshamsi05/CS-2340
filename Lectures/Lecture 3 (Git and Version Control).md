Version Control System
- VCS
	- tracks changes in computer files
	- coordinate work between multiple developers
	- Who made what changes and when
	- revert changes at any time

Why Version Control
- allows for easy collaboration making software development in a team environment a lot simpler
- allows for storage, access, and restoration by giving a clear auditable history of the project

Git vs Github
- Git is command line tool
- Github allows users to use git more easily

General Workflow
- check that you are up to date with Remote Repo
- retrieve changes
- make changes on local repo
- check status of local changes
- add any changes you want to staging area
- Commit changes in staging area
- Update the remote repo with your changes

Process of updating files in the repo
- make any changes to the files
- git add "file name"
	- puts file from working directory to the staging area
- git commit -m "message"
	- puts file from staging to local repo
- git push 
	- puts file into remote repository
- Always use git fetch before making any changes to make sure you are up to date
- Always use git pull before committing
	- combination between fetch and merge

Branching
- The main branch everyone has access to is the master branch
- Create a branch when wanting to make changes without affecting the main code
	- how to create a branch : git branch "Branchname"
	- going to the branch: git checkout "branchname"

Merging
- allows you to merge the branch into the main branch and carryout the changes
- Two merge 2 branches do the following
	- 1) git checkout "branchname"
	- 2) git merge "branchname"
- can make a branch from a branch

Cherrypicking
- can go back to a previous state of the code
	- git cherry-pick "tagname"
	- git log will also display 

Pull Request
- tool to aggregate branch changes and for others to check to see if its worthy of being merged into the main branch

Branch protection
- Goal: do not want anyone to change the main directly
- Need Github pro

