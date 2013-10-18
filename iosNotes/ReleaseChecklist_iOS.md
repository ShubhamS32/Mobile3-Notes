##Checklist before release

A) Check the upgradation from older version to new version.
B) Check the all functionality after upgradation.
C) Make appropriate changes in constant.h for live URL’s.
D) Change code signing to distribution.
E) Edit the scheme to release from debug.
F) Change the current Bundle version.
Build Setting -> Target -> summary -> version and build
or 
change in the  -Info.plist file  property “Bundle version”
G) Update the current version to iTunes connect with appropriate information and screenshots. 


##Checklist after the release

1) Commit and push the stable code in the present working branch for Headsup and checkin library.

	$ git add .
	$ git commit -m “comments”
	$ git push origin presentbranch

2) Create the new branch with release version i.e release2.0,
      if doing for  checkin library i.e  headsup/release2.0.

	$ git branch newbranch

3) Now push the code from working branch to release branch 

	$ git push origin newbranch
       -u when you push code for first time

4)  Switching to release branch 
	$ git branch checkout newbranch 

5) Merge the code from presentbranch to develop
	$ git branch  checkout develop
	$ git merge presentbranch
	
6) Merge the code from develop to master branch
	

###NOTE : -
- We create headsup/release2.0 for checkin library as the same library is used by other applications also.

-To check the status 
$ git status

-To check the log of commit 
	$ git log
