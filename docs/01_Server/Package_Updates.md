<style>
	h4 {
		font-weight: bold;
	}

	.code {
		font-size: 14;
		font-family: courier;
	}
</style>

<h4>Package Updates</h4>

It is highly recommended to update the server packages when there are updates available. Since we are running an Ubuntu server, the following commands will look for updates and upgrade the packages automatically, including the kernel:

<p class="code">apt-get update && apt-get dist-upgrade</p>