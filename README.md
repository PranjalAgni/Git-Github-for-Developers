# Git-Github-for-Developers
This is intro to git and github and how to use it without all the hassle

## What is git?
In programming world most of the time you are not working alone,so [git](https://git-scm.com/) is a piece of software which allows you to collaborate with others.According to git official site git is *distributed version control system*, there are many version control system out there but git is the most popular once.*Version Control* itself means keeping track of changes to your software during its lifecycle, think it like checkpoints in games when you complete a mission a checkpoint is saved which tells the next time you play that game you have to start from there, git is also like that it makes these checkpoints and you can go back to them any time you need.Infact the creator of linux kernel Linus Torvalds, is the creator of git.You can use git using command line or their gui.You can [install](https://git-scm.com/downloads) git from here.

## What is github?
Github is *Built for Developers*. It uses git internally but it adds a lot of extra features on top it like commits,forks,issues etc. Think of github as a way of managing your code with git but it's on the cloud. Github has many learning resources, I will list the popular once:
1. [Learn git by playing](https://learngitbranching.js.org/) This is very interesting resource, you don't need to setup anything all the commands are inbuilt in this and it has levels like games, which you have to complete.
2. [Github Guide](https://guides.github.com/) This is the official guide from the github teams, it is very nicely written to understand every bits and pieces.
3. [Try Github](http://try.github.io/) It lists all the resources to learn git, if you are a complete beginner go with this one.


## Configure local git with name and email
You can configure git with your name and email so it will identify you as user. When you use git for the first time it asks to setup the name and email.We will setup email and username globally so to do that:
```
 git config --global user.email "<YOUR_EMAIL>"
 git config --global user.name "<YOUR_NAME>"
```

##  Initialize a git repo on your local computer
To initalize a git repo on your local computer whether it's a pre-existing folder or a new folder which you want to make a git repo.Just navigate to that folder using command line and then run this command
```
git init
```
Yup thats it :)
Now to check whether git repo successfully initalized:
1. *Windows* ```dir /ah```
2. *Mac*  ```ls -d. *```
3. *Ubuntu* ```la -a```

You will see a directory named ```.git``` it is hidden from us, because we don't need to touch it and all the tracking,logs,rollbacks is stored here. If you are interested in how git works, which data structures it uses internally you can go [here](https://www.atlassian.com/git/tutorials/advanced-overview). It is interesting to see how git uses tree,hashmaps internally :wink: 	 


##  Check the status of a git repo
You can check which files are tracked by git and which are not using this command:
```
git status
```
This will list two type of files, those which are tracked will be shown in green and files which you added currently or untracked files are shown in red.To understand it more deeply git uses a tree data structure called Working Directory, this tree syncs with filesystem of your local git repo and as soon as you add,modify files it tracks it.





