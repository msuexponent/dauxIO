## Theme Updates

To check for theme updates, you will need the Foundation gem installed on the client (your computer):

```
gem install foundation
```

Now you can run this command in your theme directory:

```
foundation update
```

This will fetch the latest version of Foundation as per the release in your Gruntfile. After the update, you will need to rebuild all the theme assets:

```
fnpm run build
```
