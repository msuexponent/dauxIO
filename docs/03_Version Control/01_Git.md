<style>
	.code {
		font-size: 14;
		font-family: courier;
	}
</style>

<h4>Git</h4>

When you use Git, the workflow generally is toward version control only. You have a local repository where you work and a remote repository where you keep everything in sync and can work with a team and different machines. But you can also use Git to move your application to production. To begin, clone the repository on the client (your computer):

<p class="code">git clone ssh://root@msuexponent.com/var/repo/site.git msuexponent</p>

This will clone the theme directory into a folder called msuexponent, which can then be placed in the wp-content/themes folder in a typical WordPress setup. 

To make a commit, run the following commands:
<p class="code">git add .</p>
<p class="code">git commit -m “Commit message goes here”</p>
<p class="code">git push</p>