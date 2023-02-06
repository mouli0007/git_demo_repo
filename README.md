################Git and GitHub Work Flows Comcepts #######################


GIT  => Is a tool to track your code overtime by 
maintaining the previous version and updating the new version


GitHub => A Website to host your reposiories online


GIT Commands !

1=> Clone => Bringing a repository to your local machine from github
add => Track your file changes in GIT
commit =>Save Your files in GIT
Push =>Upload Git Commits to a remote repo, like github

git status => to check the status of our code changes and shows you the modified file 

Once (git add .) is done your files are ready to be commited

git commit -m (random message ) => to commit locally

git push =>  to push our code from local machine to remote reposiory


###############################
##############################

Creating SSSH Keys 

CMD => ssh-keygen -t rsa -b 4096 -C "mouli0007@github.com"

click enter 2 time => skipping the phrase name = > it will generate a random key 

ls  = > to get ur key {

It Will Provide you 2 key 
1=> testKey(PRIVATE)
2=> testkey.pub(PUBLIC_KEY)
}


cat testkey.pub => to view your public key

pbcopy < testKey.pub=> copies to our clipboard


###########################
#####################
######################

#################Git Branching !###########################


Types of Branches !

 1=> Master Branch !
 2 => Feature Branch !
3=> Hot Fix Branch !


Commands !

git branch=> To check in which branch you are in 
git checkout -b (name of your branch)=> git checkout -b feature-readme-instructions
git merge => merging two branches
git diff (branch name) => compares old and new versions of the code
git pull = > making a pull request from a specific branch you want 
git branch -d (branch name) => to delete a specific branch



(You cant switch to different branches 
if u have smae code both in main and sub-branches it may overwritten)

#######=> You can use STASH to hold your code for some time ! and we can retrive it later

####################
#############################

#############Merge Conflicts !####################


######2 ways to fix merge conflicts !

1=> In Terminal
2=>Directly in Code editor(Easiest way to do that !)


######### UNDOING IN GIT #################

Example-One: If you want to undo the changes in Stagging (git add .)

Commands !

1=> git reset
###or###
2=> git reset (file name)

3=>git status (to view your changes !)

#####
Example-Two: If you want to undo the changes in Commits(git commit.)


Commands ! 

=>git reset HEAD~1 (Takes you to the previous commit and undo the recent commit you have made)
=> git log (To See All Your Commits in cronological order )


#########

Example-Three: If you want to change or undo for any specific commit

Commands !

=> git reset (commit id/commit hash)


#########

Example-four: If you want to completely remove your any specific commit

Commands !

=> git reset --hard (commit id/commit hash)




######################  Defenitions ! ################################


GIT Fork ..? 


A fork is a copy of a repository that you manage. 
Forks let you make changes to a project without affecting the original repository. 
You can fetch updates from or submit changes to the original repository with pull requests.

What is a pull request used for Git?


Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. 
Once a pull request is opened, you can discuss and review the potential changes with collaborators
 and add follow-up commits before your changes are merged into the base branch.
 
 
 What is Git branching and merging?
 
 
Image result for what is git branching
Merging Branches. Once you've completed work on your branch, 
it is time to merge it into the main branch. 
Merging takes your branch changes and implements them into the main branch. 
Depending on the commit history, 
Git performs merges two ways: fast-forward and three-way merge.


What is the use of git stash?


Use git stash when you want to record the current state of the working directory and the index, 
but want to go back to a clean working directory. The command saves your local modifications away 
and reverts the working directory to match the HEAD commit.
