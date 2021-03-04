Push - being able to upload stuff from a local repository to a remote repository. This is how you transfer commits from local repository to remote.
If someone were to change something on their local repo, and they want everyone else to see the changes, they push it to the remote repo. An example is below: 
git checkout master
git fetch origin master
git rebase -i origin/master
# whatever you are changing
git push origin master
In this example you want to fetch the master to make sure it is up to date, rebasing the changes on top of them, and pushing it
