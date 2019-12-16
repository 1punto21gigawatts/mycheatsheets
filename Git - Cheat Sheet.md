# Git - Cheat sheet



------

| Add files and commit                       | Description                                                |
| ------------------------------------------ | ---------------------------------------------------------- |
| git status                                 | Checking status of current git folder.                     |
| git add <filename>                         | Adding a single file commit.                               |
| git add --all                              | Add all new files and folders for commit. *                |
| git commit -a -m "<message>"               | Commiting all changes with a comment.                      |
|                                            |                                                            |
| **Push changes**                           |                                                            |
| git push                                   | Push to the default remote repository.                     |
| git push -u origin master                  | Push from origin(local) to master(git server).             |
| git remote add origin <serveraddress>      | Setting up the remote push server (master).                |
|                                            |                                                            |
| **Branching**                              |                                                            |
| git checkout -b example                    | Create new branch called example and switch to it.         |
| git checkout master                        | Switch back to master.                                     |
| git branch -d example                      | Delete branch example.                                     |
| git push origin <brachname>                | Pushing the branch to the remote repo.                     |
|                                            |                                                            |
| **Update & Merge**                         |                                                            |
| git pull                                   | Update local repo to latest commit from remote.            |
| git diff <sourcebranch> <targetbranch>     | Previewing changes of two branches.                        |
| git merge <branch>                         | Merge another branch to your active branch.                |
|                                            |                                                            |
| **Logs**                                   |                                                            |
| git log --pretty=oneline                   | A nice way to view log.                                    |
| git log --graph --oneline --decorate --all | Tree view of log.                                          |
|                                            |                                                            |
| **Help**                                   |                                                            |
| git --help                                 | Not sure what this does.                                   |
|                                            |                                                            |
| **.gitignore**                             |                                                            |
| .gitignore                                 | Create this file with a list of files to exclude from git. |
|                                            |                                                            |

`* Note this does not add empty folders.`