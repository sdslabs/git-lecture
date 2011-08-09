#Git Lecture Notes

##Topics Discussed
* SSH, public key authentication.
* Version Control
* Git Basics
* Git Workflow
* Github
* Extra git commands
* Git GUI's

##SSH

###Installing ssh
`sudo apt-get install openssh`
###Connecting to server
`$ ssh username@hostname`
###Public key authentication
`ssh-keygen -t rsa`
The private key is at `~/.ssh/id_rsa` while the private key is at `~/.ssh/id_rsa.pub`
The server needs your public key to authenticate the connection.

##Version Control
* central VCS v/s Distributed VCS
* Why Version Control 
  - Helps remember history of project
  - Move back and forth in history
  - Any break in code can be fixed easily
  - Any bugs introduced can be traced back to the code that made it
* Examples : svn, cvs, mercurial, bzr, etc

##Git Basics
This is just a simple walkthrough. You are encouraged to try out these steps on your own.

- `git init` creates a new repository
- `git add <filename>` adds files to index
- `git add .` adds everything to index
- `git commit` creates a commit
- `git commit -a` adds all *modified* files to the index and starts a commit
- A blank commit message aborts the commit
- `git checkout <??>` changes your working directory to a commit/tag/branch
- `git checkout -b branchname` creates a new branch and shifts to it
- `git branch` shows a list of all branches & the current branch
- `git merge branchname` merges the branch with the current branch
- `git tag` marks a tag for the current commit

##Little of git-jargon
Read more over [here](http://book.git-scm.com/7_glossary.html)

- `branch` is an active line of development.
- `commit` is a snapshot of the working directory
- `tag` is an alias of a particular commit
- `HEAD` is a pointer to the current checked out branch
- `tree` is the internal representation of working directory in git
- `blob` is the internal representation of files in git
- `index` is a staging area for the commit in progress

##Git workflow
Mainly from [here](http://nvie.com/posts/a-successful-git-branching-model/)  
Topics include branches, stable, hotfix, release, development, feature branch etc.

##Github
- <http://github.com> is an awesome site that allows people to share code, projects and colloborate easily using git.
- Create an account
- Setting up ssh-keys
- Creating repository
- Setting `remotes`
- `push`, `pull`, `fetch`, `merge`
- Github gem

##Some other things
- `git log` allows you to see your history
- `git log --oneline` gives single line history
- `git log --pretty` gives better output
- `git log --graph` shows your commit graph
- Git GUI Systems - `gitg`, `git-cola`, `qgit`, `giggle` and the windows git-gui as well.
- `.gitignore` file to store system specific stuff (configuration, databases, temp files, cache, build)

##Redmine
- Create user accounts
- `git config user.name` and `git config user.email` should be setup
- Pass along the public keys (via email)

#Resources on Git
* [Git Cheat Sheets & Excellent starting guide](http://help.github.com/git-cheat-sheets/)
* [Everyday GIT With 20 Commands Or So](http://www.kernel.org/pub/software/scm/git/docs/everyday.html)
* [Pro Git Book](http://progit.org/book/)
* [Git Reference](http://gitref.org/)
* [Git Tutorial](http://www.kernel.org/pub/software/scm/git/docs/gittutorial.html)
* [Git Community Book](http://book.git-scm.com/)
* [Another git tutorial](http://www.ralfebert.de/tutorials/git/)
* [Git beginner tutes](http://sixrevisions.com/resources/git-tutorials-beginners/)
* [Git for Computer Scientists](http://eagain.net/articles/git-for-computer-scientists/) 
* [Git from bottom up](http://ftp.newartisans.com/pub/git.from.bottom.up.pdf)
