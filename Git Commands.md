
![Log](http://media.w3guy.com/wp-content/uploads/2015/02/git.jpg)


# Gitgub commands with SSH:

## Generate an SSH key :

1- Go to your profile and click on the SSH and GPG keys

2- Click on New SSH key to generate an SSH key for your account

## Connect to SSH 

1- Open your GitBash terminal 

2- type : ```ssh -T git@github.com ```

   if you see a welcome note with your account name means that the connection is alreay established
   
3- Clone a repository using SSH

``` git clone git@github.com:nairuzabulhul/General-Commands.git (path of your repository)```

note: the path can be found by clicking the green button Clone or Download. you will #Clone with SSH 


## Working with the clone repository :

- Once you clone your repositroy, cd to the direcotry 

``` cd nameOFyourRepo ```



# Github Commnads 

1- Create a local repository 
   
   mkdir newrepo

2- cd to that newrepo
  cd newrepo
  
3- inside the newrepos, initialize a git gile
  - git init
  
4- Add files to the direcotry 

5-  Check the added files 

    git status

6- Add them to git 
  git add name of file
  
7- Commit the changes

  git commit -m "initial commit"
  
8- Push the chnages 
 
  git push --set-upstream origin master

  
Get the repo

Just clone it:
GitHub: git clone git@github.com:YOUR_USERNAME/REPO_NAME.git
BitBucket: git clone git@bitbucket.org:USERNAME/REPO_NAME.git  

Committing the changes after updating the files:
git commit -a -m "your comment"

push the files to the exsiting repo

git push


## BitBucket Commands:
- hg pull
- hg status
- hg commit -m "Updates"
- hg push 
