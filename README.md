# Dev_Ops_Lab1
Lab 1 for cloning and working with repositories

## LAB-1 GIT COMMANDS

### 1. Clone the repository:
```sh
git clone https://github.com/Shashwat-Tripathi-GITHUB/Dev_Ops_Lab1.git
```

![Project Screenshot](./images/Git%20clone.png)


### 2. Adding image:
```sh 
git add .
git commit -m "my first commit with image"
git push
```

![Project Screenshot](./images/git%20push%20image.png)


### 3. Git status and Diff Commands:
```sh 
git staus
```
![Project Screenshot](./images/git%20status.png)

```sh
git diff
```
![Project Screenshot](./images/git%20diff.png)

```sh
diff diff && git status
```
![Project Screenshot](./images/git_diff_vs.png)


## LAB-2 GIT COMMANDS
### 1. Checking the logs
### version1:
```sh
git add hello.txt
git commit -m "v1"      
```
![Project Screenshot](./images/lab2_1.png)

### version2:
```sh
git add hello.txt
git commit -m "v2"      
```
![Project Screenshot](./images/lab2_2.png)

### version3:
```sh
git add hello.txt
git commit -m "v3"      
```
![Project Screenshot](./images/lab2_3.png)

```sh
git log
```
![Project Screenshot](./images/lab2_4_git_log.png)


### 2. Creating branch and merging with Main
```sh
git branch feature1
git add .
git commit -m "feature commit 1"
git push origin feature1
```
![Project Screenshot](./images/lab2_5_feature1.png)

### Merged with Main
```sh
git add README.md
git commit -m "Updated README before merging"


git checkout main
git merge feature1 -m "Merging feature1"
```
###### Image 1
![Project Screenshot](./images/lab2_6.png)
###### Image 2
![Project Screenshot](./images/lab2_7_git_merge.png)
###### Image 3
![Project Screenshot](./images/lab2_8.png)

## Lab-3 Submodules
#### This is the Repository with the Submodules Experiment.
https://github.com/Shashwat-Tripathi-GITHUB/Main_Submodules

## LAB-4 SUBVERSION
### Installation of Subversion (SVN) using Homebrew:
```sh
brew install subversion
```
![Project Screenshot](./images/image11.png)

### Creating repo:
```sh
mkdir -p ~/svn-repos/myrepo
svnadmin create ~/svn-repos/myrepo
```

### Configure svnserve:
```sh
nano ~/svn-repos/myrepo/conf/svnserve.conf
```

### Start svnserve:
```sh
svnserve -d -r ~/svn-repos
```
### setting up password:
![Project Screenshot](./images/image12.png)

### starting server and verifying:
![Project Screenshot](./images/image13.png)


