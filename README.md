# git_basic_commands

Git is the most commonly used version control system. Git tracks the changes you make to files, so you have a record of what has been done, and you can revert to specific versions should you ever need to. Git also makes collaboration easier, allowing changes by multiple people to all be merged into one source.

Git basics commands

<pre>git init
git status 
git log
git add <file_name> 
git add . ==>add all files
git commit -m "required msg"
git pull origin <branch_name>
git push origin <branch_name>
git checkout -b <new_branch_name> ==> will checkout to given new_branch_name
git branch <branch-name>
git branch -d <branch_name>
git merge <dest_bn> <src_bn></pre>


<pre><b>git help</b>  </br>
Take help from github help section for different commands and other errors.</pre>

<pre><b>git init </b>  </br>
To create a local git repository for us in our store folder.This will help to manage the git commands for that particular repository.

<b>git status </b>  </br>
To see whats changed since last commit.It shows all the files that have been added and modified and ready to be commmitted and files which are untracked

<b>git config </b>  </br>
To set the basic configurations on github like your name and email.

<b>git config –global user.name “Yourname” </b>  </br>
Sets configuration values for your user name on git.

<b>git config –global user.email Yourmailid@gmail.com</b>  </br>
Sets configuration values for your user email on git.

<b>git add Readme.txt</b>  </br>
To add a file Readme.txt to the staging area to track its changes.

<b>git commit -m “Created a Readme.txt” </b>  </br>
To commit our changes(taking a snapshot) and providing a message to remember for future reference.

<b>git log </b>  </br>
To check the history of commits for our reference.

<b>Different ways to use add command:</b>  </br>

<b>git add</b>  </br>
To add a specific list of files to staging area.

<b>git add --all</b>  </br>
To add all files of current directory to staging area.

<b>git add *.txt</b>  </br>
To add all text files of the current directory to staging area.

<b>git add docs/*.txt</b>  </br>
To add all text files of a particular directory(docs) to staging area.

<b>git add docs/</b>  </br>
To add all files in a particular directory(docs) to staging area.

<b>git add “*.txt”</b>  </br>
To add text files of entire project to staging area.

<b>git diff</b>  </br>
To figure out what changes you made since last commit.

<b>git reset head license</b>  </br>
To undo staging of the file that was added in the staging area.

<b>git checkout –license</b>  </br>
To Blow away all changes since the last commit of the file.

<b>git commit -a -m “Readme.md”</b>  </br>
To add any of our tracked files to staging area and commit them by providing a message to remember.

<b>git reset –soft HEAD^</b>  </br>
To undo last commit and bring file to staging area.

<b>git reset –hard HEAD^</b>  </br>
To undo last commit and remove file from the staging area as well(In case we went horribly wrong).

<b>git reset –hard HEAD^^</b>  </br>
To undo last 2 commits and all changes.

<b>git remote add origin https://github.com/nidhisri99/git_basic_commands.git</b>  </br>
This commands make a bookmark which signifies that this particular remote refers to this URL. </br>
This remote will be used to pull any content from the directory and push our local content to the global server.</br>

<b>git remote add <address> </b>  </br>
To add new remotes to our local repository for a particular git address.

<b>git remove rm</b>  </br>
To remove a remote from our local repository.

<b>git push -u origin master</b>  </br>
To push all the contents of our local repository that belong to master branch to the server(Global repository).

<b>git clone https://github.com/nidhisri99/git_basic_commands.git</b>  </br>
To clone or make a local copy of the global repository in your system
(git clone command downloads the repository and creates a remote named as origin which can be checked by command – git remote -v).

<b>git branch Testing</b>  </br>
To create a new branch named as Testing.

<b>git branch</b>  </br>
To see all the branches present and current branch that we are working on.

<b>git checkout Testing</b>  </br>
To switch to branch Testing from master branch.

<b>ls</b>  </br>
To see directories and files in the current directory.

<b>git merge Testing</b>  </br></b>  </br>
To merge Testing branch with master branch.

<b>git branch -d Testing</b>  </br>
To delete Testing branch.

<b>git checkout -b admin</b>  </br>
To create a new branch admin and set it as current branch.

<b>git branch -r</b> </br>
To look at all the remote branches.

<b>git branch -D Testing</b>  </br>
To forcefully delete a branch without making commmits.

<b>git tag</b>  </br>
To see the list of available tags.

<b>git checkout v0.0.1</b>  </br>
To set the current tag to v0.0.1.

<b>git tag -a v0.0.3 -m “version 0.0.3”</b>  </br>
To create a new tag.

<b>git push –tags</b>  </br>
To push the tags to remote repository.

<b>git fetch</b>  </br>
To fetch down any changes from global repository to current repository

<b>git rebase</b>  </br>
Three tasks are performed by git rebase

Move all changes to master which are not in origin/master to a temporary area. </br>
Run all origin master commits.</br>
Run all commits in the temporary area on top of our master one at a time, so it avoids merge commits.</br>
</pre>
