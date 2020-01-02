Git Commands 
++++++++++++++++++
- git config
-- git config --global user.name "YOURNAME"
-- git config --global user.email "YOUREMAIL"

- git init
( initialize git repo to current directory ) ( added hidden file .git )

- git status ( check new files )
- git add filename (OR) git add .
- git commit -m "YOUR COMMIT"
- git log  
- git log pretty=oneline ( You will get HEAD id )
- git checkout "YOUR HEAD ID"
- git checkout master ( Your main proj )
- git tag 0.1.0
- git branch
- git branch BRANCHNAME ( create new branch )
- git checkout YOURBRANCHNAME ( switch working directory )
- git merge YOURSUBPROJECTFOLDER ( pull from edited project to main project ) ( In main project ) 
______________________
- git clone <SOURCE REPO>  <CLONE REPO>
- git pull origin master 
-- git remote show origin ( ORIGINAL REPO )
-- git push 
( can't sent clone repo to original repo but original to clone can. )

BARE REPO
============
mkdir central
cd central
- git init --bare
- git clone <CENTRAL> <APP1> ( For developer 1 )
- git clone <CENTRAL> <APP2> ( For developer 2 )
- git push origin master ( From developers to CENTRAL )
- git pull origin master ( Pull Central to Developer )

GIT PUSH ERROR ( WARNING )
first update and push ( method ) 
You will get confilct if other developer also edit this file and upload.
Save your method and COMMIT Updated file.
- git confilct resolve
- git log -pretty=oneline

UPLOADING GITHUB
==================
- git remote show origin
- git remote remove origin
- git remote add origin "YOUR GITHUB LINK" 
( Add readme.md )
- git add .
- git commit -m "added readme.md"
- git push origin master ( Need Username and Password )

Git error: “Please make sure you have the correct access rights and the repository exists”
ြဖစ်နေခဲ့ရင် 
- git remote set-url origin git@yourGitUrlHere
