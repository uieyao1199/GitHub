# Basic github setup

## Introduction

In this part, you can test your jupyter notebook on EC2 virtual machine.

## Create repository

* Go to you github account, click __repositories__:
<img src='image/rep.png'>

* Click on __New__:
<img src='image/new.png'>

* Type in your repository name(could be any name you want, usually we use the project name) and you can check the checkbox of creating a README file which is highly reommanded.
<image src='image/create.png'>

## Connect your project and the repository

* Open a __terminal__ and change the directory to the project folder on you computer.

* Here is an example:
```
FandeMacBook-Pro:~ fanliang$ cd Desktop/github_file/Richard/test2/test_rep/
FandeMacBook-Pro:test_rep fanliang$ ls
README.md	image
```

* __Note__: This is an exampe on my computer, you can test this any of your previous project folder.

* Add remote to the folder(git@github.com:globalaiorg/test_rep.git. This is the repository address of mine, you will have your own project repository):
```
FandeMacBook-Pro:test_rep fanliang$ git init
Reinitialized existing Git repository in /Users/fanliang/Desktop/github_file/Richard/test2/test_rep/.git/
FandeMacBook-Pro:test_rep fanliang$ git remote add origin git@github.com:globalaiorg/test_rep.git
```

* Check status:
```
FandeMacBook-Pro:test_rep fanliang$ git remote -v
origin	git@github.com:globalaiorg/test_rep.git (fetch)
origin	git@github.com:globalaiorg/test_rep.git (push)
```

* Basic [git command](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)

* Tips:
  1. Always use `git pull` before you push.
  2. Order of push:`git add [file_name]`(or `git add *`which will add all files that are not in repository). `git commit -m 'command'` adding command of the files you want to push. `git push -u origin master` pushing to repository.
