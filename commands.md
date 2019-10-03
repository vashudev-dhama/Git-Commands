>CONFIGURE GIT USERNAME AND EMAIL FOR FIRST TIME ON PC:

Open git bash and run the following commands:
```
$ git config --global user.name <User Name>
$ git config --global user.email <Email id>
```
You can check your configurations by:
```
$ git config --list
```
>FOR UPLOADING YOUR EXISTING PROJECT ON GITHUB:
1. Create a new repository for your project on your github account and copy the link of the repository.

2. Open git bash in your pc.

3. Run following commands:

```
$ cd /<project-path>
$ git init
$ git remote add origin https://github.com/USERNAME/REPOSITORY.git
$ git add .
$ git commit -m "any msg"
$ git push origin master
```
***Note: You can always skip the add and commit of a type of file/s by including the .extension of that type of file/s in .gitignore file.***
>FOR UPDATING YOUR WORK ON A PROJECT WHICH YOU ALREADY HAVE ON GITHUB:
1. Save your work
2. Open git bash
3. Run following commands:
```
$ cd /project_path
$ git add .
$ git commit -m "any msg"
$ git pull origin master
$ git push origin master
```
>SOME OF THE BASIC AND IMPORTANT GIT COMMANDS:

To clone a repository:
```
$ git clone https://github.com/USERNAME/REPOSITORY.git
```
To add file/s for next commit version:
```
$ git add <file-name>
or
$ git add .
```
To save the current track of the repository:
```
$ git commit -m "message"
```
To see what's currently going on, on your repository:
```
$ git status
```
To send/publish the changes to github:
```
$ git push
```
To download the latest changes made to the repository by some other contributor/s (if any):
```
$ git pull
```
To list the commits made so far:
```
$ git log
```
To reset your whole repository back to a certain version:
```
$ git reset --hard <commit-hash>
or
$ git reset --hard origin/master
```
To list out the changes made till current version of repository:
```
$ git reflog
```
To change a remote's URL:
```
$ git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```
To verify the remote URL:
```
$ git remote -v
```
>BRANCHING:

List all branches of repo:
```
$ git branch
```
Add a new branch:
```
$ git branch <feature-branch>
```
Move to other branch:
```
$ git checkout <feature-branch>
```
Push the new branch:
```
$ git checkout <feature-branch>
$ git push --set-upstream origin <feature-branch>
```
Merge the branch with master branch:
```
$ git checkout master
$ git merge <feature-branch>
```