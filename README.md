# git-workshop
Simple repository for the Git 101 Workshop given to UC Berkeley students

## Part 1 - Setup and Prep
* Create a github account or login to your account if you don't have one
* Make sure that you have git installed
 * https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
 * Mac - Download directly or install through brew
 * Windows - download from http://msysgit.github.io/ and install
 * Linux - use apt-get or yum
 * https://gist.github.com/derhuerst/1b15ff4652a867391f03
 
## Part 2 - Local repo
* Initialize git repo
```
git init
git status
```

* Add a file and commit
```
git add file1.txt
git status
git commit -m "adding file1.txt"
```
  
* Add multiple files  
```
git add *.txt 
git commit "Adding many files"
```
* History 
 ```
 git log
 git log --summary
 ```
 
## Part 3 - Remote repository

* Push to empty repo

 ```
 git remote add origin https://github.com/annjose/empty.git
 ```
* Clone the repo of HTML workshop
```
 * git clone https://github.com/annjose/hack-into-it-2017-web.git
 * git status
 * git log
 * git remote show origin
 ```
 
## Part 4 - Branching & Merging
* Create new branch
```
 * git branch my-branch
 * git checkout my-branch
```

* Make changes in the new branch
 ```
 * git add myfile.txt
 * git commit -m "Adding my file"
 ```
 
* Merge my-branch to  master
```
 * git checkout master
 * git merge my-branch
 * git push
 * git branch -d my-branch
 ```
 
## Part 5 - Pull Requests

```
 * git branch new-feature
 * git checkout new-feature
 * make changes
 * git push origin new-feature
 ```
 * Go to gihub.com and create a PR
 * Note: Choose the base repo correctly
