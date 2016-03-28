<style>
	.code {
		font-size: 14;
		font-family: courier;
	}
</style>

<h4>Git Flow</h4>

Git Flow is a git branching and release management strategy that helps developers keep track of features, hotfixes and releases in bigger software projects. You will need to have the git flow extension installed on the client (your computer) before you continue.

We primarily use the feature branch to work on code in isolation from the develop branch:
<p class="code">git flow feature start featureNameHere</p>
<p class="code">git add .</p>
<p class="code">git commit -m “Commit message”</p>
<p class="code">...</p>
<p class="code">git add .</p>
<p class="code">git commit -m “Final commit message”</p>
<p class="code">git flow feature finish featureNameHere</p>

Upon completing the feature, the branch will be merged with develop and you can then merge develop with the production master branch after running tests.