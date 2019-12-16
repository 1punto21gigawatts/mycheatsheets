# Git - Creating a new repo



------

### Pre-requisites 

Use git with ssh key pairs.  Copy public key data into your Git account (Github,  Gitlab, etc..) 
Install Git on the local machine. Via Yum, Dnf, Apt etc... 

------

##  Create new repo from scratch 

- Create a directory to contain the project. 

- Go into the new directory. 

- Type 

  ```bash
  git init
  This initializes the current folder for git usage.
  ```

- Write some code/ update some files/ add some files. 

- Add a ".gitignore" file in the root of the folder you are in.

  ```bash
  vi .ignore
  
  Within this file, list files or folders you want ignored.
  E.g.
  log/
  morelogs/
  garbage.txt
  ```

- Type "git add".

  ```bash
  git add filename
  or
  git add * (to add all files from current folder and recursively into sub folders)
  ```

  If you have an existing folder with files then use the "git add *" option initially.

- Type git commit. 

  ```
  git commit -a -m "some comment"
  This will add all files being tracked or in git repository and add a comment. Without a comment it will not commit.
  ```

  

##  Connect it to Github or other Git service 

 You’ve  now got a local git repository. You can use git locally, like that, if  you want. But if you want the thing to have a home on github/git service, do the following. 

- Go to github/git service.

- Log in to your account. 

- Click the new repository/project button. You’ll have an option there to initialize the repository with a README file, but don’t select this. 

- Click the “Create repository/ Project name” button.

- Give it a name and change the owner to groups or specific users.

- Change the Visibility level. In this case we'll choose "Internal"

- Choose Create

- Type the following:

  ```bash
  $ git remote add origin your-git-url-here 
  ```

- Type the following:

  ```bash
  $ git push -u origin master
  ```

  