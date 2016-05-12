## Grunt and Bower

Grunt is a task-based build tool which automates often mundane tasks such as minification, compilation, unit testing, etc. After configuring the Gruntfile, you can do most of that mundane work without much effort. 

Bower works by fetching and installing packages from all over, taking care of hunting, finding, downloading, and saving the stuff you’re looking for. Bower keeps track of these packages in a manifest file, bower.json.

While you're working on theme development, run this command before editing any files: 

```
npm run watch
```

If an asset fails to build or you wish to rebuild all the assets, run:

```
npm run build
```