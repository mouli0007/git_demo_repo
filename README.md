// Git and GitHub 


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
