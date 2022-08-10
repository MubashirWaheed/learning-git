# Git commands

git clone &lt;repo-url&gt;

git add &lt;file-name&gt;

git add .

git commit -m &lt;message&gt;

git push &lt;remote-name&gt;&lt;branch-name&gt;

// adds remote
git remote add &lt;remote-name&gt; &lt;repo-url&gt;

git log --oneline --decorator --graph --all

git remote -v

git remote show

// lists all the branches
git branch

// To see the last commit on each branch
git branch -v

// creates branch without switching
git branch &lt;branch-name&gt;

// creates adn switch to the created branch
git checkout -b &lt;branch-name&gt;

// delete branch locally
git branch -d &lt;branch-name&gt;

// delete remote branch
git push origin --delete &lt;branch-name&gt;

// get the tracking branch data and imediately erge with the local branch
git pull

// only fetched the data from remote tracking branch
---issue1---issue2----issue3----issue4
\
 ----issue5----issue6
git fetch

there are two main ways to integrate changes from one branch into another: the merge and the rebase

// rebasing
$ git checkout experiment
$ git rebase master
First, rewinding head to replay your work on top of it...
Applying: added staged command
$ git checkout master
$ git merge experiment
