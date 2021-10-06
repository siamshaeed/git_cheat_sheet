##git cheat sheet

<p>A distributed version control system is a system that helps you keep track of changes you've made to files in your project.

This change history lives on your local machine and lets you revert to a previous version of your project with ease in case something goes wrong.

Git makes collaboration easy. Everyone on the team can keep a full backup of the repositories they're working on on their local machine. Then, thanks to an external server like BitBucket, GitHub or GitLab, they can safely store the repository in a single place.

This way, different members of the team can copy it locally and everyone has a clear overview of all changes made by the whole team.
</p>

<h2>How to check your Git configuration:</h2>
<p>The command below returns a list of information about your git configuration including user name and email:</p>
<pre>
  git config -l
</pre>

<h2>How to setup your Git username:</h2>
<p>With the command below you can configure your user name:</p>
<pre>
  git config --global user.name "siam"
</pre>

<h2>How to setup your Git user email:</h2>
<p>This command lets you setup the user email address you'll use in your commits.</p>
<pre>
  git config --global user.email "siam@gmail.com"
</pre>

<h2>How to cache your login credentials in Git:</h2>
<p>You can store login credentials in the cache so you don't have to type them in each time. Just use this command:</p>
<pre>
  git config --global credential.helper cache
</pre>

<h2>How to initialize a Git repo:</h2>
<p>Everything starts from here. The first step is to initialize a new Git repo locally in your project root. You can do so with the command below:</p>
<pre>
  git init
</pre>

<h2>How to add a file to the staging area in Git:</h2>
<p>The command below will add a file to the staging area. Just replace filename_here with the name of the file you want to add to the staging area.</p>
<pre>
  git add filename_here
</pre>

<h2>How to add all files in the staging area in Git</h2>
<p>If you want to add all files in your project to the staging area, you can use a wildcard . and every file will be added for you.</p>
<pre>
  git add .
</pre>

<h2>How to check a repository's status in Git:</h2>
<p>This command will show the status of the current repository including staged, unstaged, and untracked files.</p>
<pre>
  git status
</pre>

<h2>How to commit changes with a message in Git:</h2>
<p>You can add a commit message without opening the editor. This command lets you only specify a short summary for your commit message.</p>
<pre>
  git commit -m "your commit message here"
</pre>

<h2>How to commit changes (and skip the staging area) in Git:</h2>
<p>You can add and commit tracked files with a single command by using the -a and -m options.</p>
<pre>
  git commit -a -m"your commit message here"
</pre>

<h2>How to see changes made before committing them using "diff" in Git:</h2>
<p>You can pass a file as a parameter to only see changes on a specific file.
git diff shows only unstaged changes by default.
We can call diff with the --staged flag to see any staged changes.
</p>
<pre>
  git diff
  git diff all_checks.py
  git diff --staged
</pre>

<h2>How to see your commit history in Git:</h2>
<p>This command shows the commit history for the current repository:</p>
<pre>
  git log
</pre>

<h2>How to see your commit history including changes in Git:</h2>
<p>This command shows the commit's history including all files and their changes:</p>
<pre>
  git log -p
</pre>

<h2>How to see a specific commit in Git:</h2>
<p>This command shows a specific commit.
Replace commit-id with the id of the commit that you find in the commit log after the word commit.</p>
<pre>
  git show commit-id
</pre>

<h2>How to remove tracked files from the current working tree in Git:</h2>
<p>This command expects a commit message to explain why the file was deleted.</p>
<pre>
  git rm filename
</pre>

<h2>How to rename files in Git:</h2>
<pThis command stages the changes, then it expects a commit message.></p>
<pre>
  git mv oldfile newfile
</pre>

<h2>How to revert staged changes in Git:</h2>
<p>You can use the -p option flag to specify the changes you want to reset.</p>
<pre>
  git reset HEAD filename
  git reset HEAD -p
</pre>

<h2>How to amend the most recent commit in Git:</h2>
<p>git commit --amend allows you to modify and add changes to the most recent commit.</p>
<pre>
  git commit --amend
</pre>

<h2>How to rollback the last commit in Git:</h2>
<p>git revert will create a new commit that is the opposite of everything in the given commit.
We can revert the latest commit by using the head alias like this:</p>
<pre>
  git revert HEAD
</pre>

<h2>How to rollback an old commit in Git:</h2>
<p>You can revert an old commit using its commit id. This opens the editor so you can add a commit message.</p>
<pre>
  git revert comit_id_here
</pre>

<h2>Branch</h2>
<h2>How to create a new branch in Git:</h2>
<p>By default, you have one branch, the main branch. With this command, you can create a new branch. Git won't switch to it automatically – you will need to do it manually with the next command.</p>
<pre>
  git branch branch_name
</pre>

<h2>How to switch to a newly created branch in Git:</h2>
<p>When you want to use a different or a newly created branch you can use this command:</p>
<pre>
  git checkout branch_name
</pre>

<h2>How to list branches in Git:</h2>
<p>You can view all created branches using the git branch command. It will show a list of all branches and mark the current branch with an asterisk and highlight it in green.</p>
<pre>
  git branch
</pre>

<h2>How to create a branch in Git and switch to it immediately:</h2>
<p>In a single command, you can create and switch to a new branch right away.</p>
<pre>
  git checkout -b branch_name
</pre>

<h2>How to delete a branch in Git:</h2>
<p>When you are done working with a branch and have merged it, you can delete it using the command below:</p>
<pre>
  git branch -d branch_name
</pre>

<h2>How to merge two branches in Git:</h2>
<p>To merge the history of the branch you are currently in with the branch_name, you will need to use the command below:</p>
<pre>
  git merge branch_name
</pre>

<h2>How to abort a conflicting merge in Git:</h2>
<p>If you want to throw a merge away and start over, you can run the following command:</p>
<pre>
  git merge --abort
</pre>

<h2>How to push changes to a remote repo in Git:</h2>
<p>When all your work is ready to be saved on a remote repository, you can push all changes using the command below:</p>
<pre>
  git push
</pre>

<h2>How to pull changes from a remote repo in Git:</h2>
<p>If other team members are working on your repository, you can retrieve the latest changes made to the remote repository with the command below:</p>
<pre>
  git pull
</pre>
