# git-command-line
Common git commands

* General

```
$ git clone https://github.com/skelkar7/example.git

$ git add .

$ git status

$ git commit -m '<version-name>'

$ git push

$ git reset --hard
```

* See difference:


$ git diff -- myfile.txt

  or if you want to see already-added changes

$ git diff --cached -- myfile.txt


* Updating GitHub forked repository:

  Add the remote, call it "upstream":

$ git remote add upstream https://github.com/whoever/whatever.git

  Fetch all the branches of that remote into remote-tracking branches,
  such as upstream/master:

$ git fetch upstream

  Make sure that you're on your master branch:

$ git checkout master

  Rewrite your master branch so that any commits of yours that
  aren't already in upstream/master are replayed on top of that
  other branch:

$ git rebase upstream/master

$ git push -f origin master