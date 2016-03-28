<style>
	.code {
		font-size: 14;
		font-family: courier;
	}
</style>

<h4>Theme Updates</h4>

To check for theme updates, you will need the Foundation gem installed on the client (your computer):

<p class="code">gem install foundation</p>

Now you can run this command in your theme directory:

<p class="code">foundation update</p>

This will fetch the latest version of Foundation as per the release in your Gruntfile. After the update, you will need to rebuild all the theme assets:

<p class="code">fnpm run build</p>