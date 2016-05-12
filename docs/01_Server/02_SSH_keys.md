## SSH keys

An SSH key is required to access the files on the server. The first step is to create the key pair on the client machine (usually your computer):

	```
	ssh-keygen -t rsa
	```

Once you have entered the SSH key generator command, you will get a few more questions:

Enter file in which to save the key (/demo/.ssh/id_rsa):
You can press enter here, saving the file to the user home (in this case, my example user is called demo).

Enter passphrase (empty for no passphrase):
You can choose whether or not to enter a passphrase here. 

Enter the following command and replace the bold text with the server’s IP address. This will copy the SSH key you just created to the server and prompt you for the root password:

	```
	cat ~/.ssh/id_rsa.pub | ssh root@[your.ip.address.here] "cat >> ~/.ssh/authorized_keys"
	```

You can now test your connection to the server using SSH:

	```
	ssh root@[your.ip.address.here]
	```