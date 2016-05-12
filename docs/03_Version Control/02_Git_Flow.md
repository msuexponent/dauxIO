## Git Flow

Git Flow is a git branching and release management strategy that helps developers keep track of features, hotfixes and releases in bigger software projects. You will need to have the git flow extension installed on the client (your computer) before you continue.

We primarily use the feature branch to work on code in isolation from the develop branch:

```
git flow feature start featureNameHere
git add .
git commit -m “Commit message”
...
git add .
git commit -m “Final commit message”
git flow feature finish featureNameHere
```

Upon completing the feature, the branch will be merged with develop and you can then merge develop with the production master branch after running tests.