<p>A distributed version control system is a system that helps you keep track of changes you've made to files in your project.

This change history lives on your local machine and lets you revert to a previous version of your project with ease in case something goes wrong.

Git makes collaboration easy. Everyone on the team can keep a full backup of the repositories they're working on on their local machine. Then, thanks to an external server like BitBucket, GitHub or GitLab, they can safely store the repository in a single place.

This way, different members of the team can copy it locally and everyone has a clear overview of all changes made by the whole team.

Git has many different commands you can use. And I've found that these fifty are the ones I use the most often (and are therefore the most helpful to remember).

So I have written them down and thought it'd be nice to share them with the community. I hope you find them useful – Enjoy.</p>

<h2>SETUP</h2>
<p>Configuring user information used across all local repositories</p>

<pre>
git config --global user.name “[firstname lastname]”
set a name that is identifiable for credit when review version history
git config --global user.email “[valid-email]”
set an email address that will be associated with each history marker
git config --global color.ui auto
set automatic command line coloring for Git for easy reviewing
</pre>

<h2>Initializing and Cloning</h2>
<p>Configuring user information, initializing and cloning repositories</p>
<pre>
git init
initialize an existing directory as a Git repository
git clone [url]
retrieve an entire repository from a hosted location via URL
</pre>
