The git / github with examples:



-the initial configuration

	git config --global user.name "Your name here": With this you can put your name so people will know who is makin gthe changes
	git config --global user.email "your_email@example.com" Whit this you will put an email that will be related to the changes made

$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager-core
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
	user.name=Antoniowtd
	user.email=antonio.rn@outlook.com
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
remote.origin.url=https://github.com/Antoniowtd/Git-and-GitHub-Markdown.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
branch.master.remote=origin
branch.master.merge=refs/heads/master

	Here we can see that I all ready have it configurated

-starting a project from zero or cloning an existing repository

	This will download the file in a folder named

	cd folder/to/clone-into/
	git clone https://github.com/gittower/git-crash-course.git

-basic workflow commands to stage and commit 

	Stage files:
	git add "Nmae of the file"
	git add README.md

	Unstage files: You can used to un stage thigs you just stage
	git reset HEAD "name of the file"
	git reset HEAD README.md

	Deleting files:
	git rm "Name of the file" you use this one to remove files
	git rm README.md

	git rm -r Git&githubmarkdown you use this one to remove folder

	Commit Files:
	git commit -m "Description of what change"
	

-push to a remote repository

	git push <remote> <branch>

git push -u origin m
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 396 bytes | 396.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Antoniowtd/Git-and-GitHub-Markdown.git
   bcc23b2..1f9d602  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

-branche: create, delete, save/commit and merge: 

	With this you will create a branch:
	git brach <branch_name>

Usuario@DESKTOP-VA1PJA4 MINGW64 ~/Desktop/Git & Github Markdown (master)
$ git branch test

Usuario@DESKTOP-VA1PJA4 MINGW64 ~/Desktop/Git & Github Markdown (test)
$ git branch
  master
* test


	With this you can delete a branch:
	git branch -d "Name of the branch"

Usuario@DESKTOP-VA1PJA4 MINGW64 ~/Desktop/Git & Github Markdown (master)
$ git branch -d test
Deleted branch test (was 1f9d602).

Usuario@DESKTOP-VA1PJA4 MINGW64 ~/Desktop/Git & Github Markdown (master)
$ git branch
* master


	With this you will move to a branch:
	git checkout <branch_name>

Usuario@DESKTOP-VA1PJA4 MINGW64 ~/Desktop/Git & Github Markdown (master)
$ git checkout test
Switched to branch 'test'
M       The_gitandgithub.md
Your branch is up to date with 'origin/master'.

	
-gitflow. 

