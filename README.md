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
