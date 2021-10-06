<p>A distributed version control system is a system that helps you keep track of changes you've made to files in your project.

This change history lives on your local machine and lets you revert to a previous version of your project with ease in case something goes wrong.

Git makes collaboration easy. Everyone on the team can keep a full backup of the repositories they're working on on their local machine. Then, thanks to an external server like BitBucket, GitHub or GitLab, they can safely store the repository in a single place.

This way, different members of the team can copy it locally and everyone has a clear overview of all changes made by the whole team.

Git has many different commands you can use. And I've found that these fifty are the ones I use the most often (and are therefore the most helpful to remember).

So I have written them down and thought it'd be nice to share them with the community. I hope you find them useful – Enjoy.</p>

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
