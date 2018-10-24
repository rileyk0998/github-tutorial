# GitHub Tutorial

_by Riley K_

---
## Git vs. GitHub
Git is the tool that you use inorder to in  Github, which is the platform where you can store your projects you make. 
#### Git
-Git keeps snapshots of the code in local repository  
-Doesn't require Github
#### Github
-Stores code in the cloud, accecable anywhere in the world  
-Saves all changes so you can see even past actions  
-Easy to collaberate on the same files with other people  
-Requiers Git  


---
## Initial Setup
**Githud & Cloud 9**
1. Start off by creating a Github account with your email (username: _`<your name>`_, if you are a HSTAT student use your HSTAT email but without the `@hstat.org`)
2. Go to [Cloud9 login](https://c9.io/login)
3. Go to the top right corner and click on the image of the cat
4. Log in and click the settings icon 
5. Go to connected services and click connect with Github
6. Go back to dashboard/workspace and create an new workspace
7. Name the workspace what ever you want (preferably what you will be doing in it)
8. Describe what this workspace if for
9. scroll to Team and seclect `don't set a team for this workspace` 
10. Template: Select `Blank`
11. Create the workspace
12. Close `README.md` tab  

**Auto Save**  
1. Go to menue(top left), then click on Cloud9, select preferences
2. Next, click experiimental, and files
3. you should see `auto save` **swich to on focus change**  

**SSH Key**
1. Go to the top right corner of Github, click on profile icon, and then settings
2. On the left side bar look for and select SSH and GPG Keys
3. Create new SSH key, title whatever you want(preferably Cloud 9)
4. Swtich to Cloud 9 in a different tab
5. At the top-right corner click on gear icon and SSH key 
6. Copy and paste 2nd SSH key into github(it should start with ssh-rsa), once you're done add the SSH key 
7. Go back to your workspace and open the workspace you plan to work in 
8. Type in `ssh -T git@github.com` 
9. It should say: `Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access._` 

**Congrates! You're finally done setting up your Github and Cloud 9 account!**


---
## Repository Setup

1. Create a directory and then `cd` into it (Type `mkdir <name>` and then `cd <name of directory>`)
2. Type in `git init` in order to initialize the directory (only do this once in the beginning of a new directory)
3. Go to Github, at top-right click the `+`, create a new repository, name it and then click `create repository` 
4. Once created, make sure the url is under SSH, then go to the second section to copy and paste the following lines on to your Cloud 9(one at a time)  
5. Now you can create a README.md file (`touch <filename>.md`) 
6. You can now type whatever you want into it. 
7. Once you're done typing save and add (`git add .`) it (file should have auto saved, if not click `CTRL S` and make sure there is a `x` and not a gray circle by the title)
8. Once it is added, type `git commit -m "<breif message of what you did>"`  


---
## Workflow & Commands
* `Git status` - used to check where you are, if you have saved anything  
* `git add --all` - add all changes and any deleted/renamed files  
* `git push -u origin master` - Only done once in the beginning when making the repository  
* `git diff` - To see changes made in file  
* `git log` - List past commits that you have recently done  


---
## Rolling Back Changes
* `rm -rf .git` - remove `git init`, this can be done if you accidentally initialized the wrong directory  
* `git checkout -- file` - Undo edits in file before add  
* `git reset HEAD file` - Undo added file  
* `git remote -v` - Where git push will send commits to. V = “verbose”  
* `git reset --hard HEAD~1` - Undos push, commit, and add. Delete code/anything that was typed into the file last.

* `git reset --soft HEAD~1` - Undos push, commit, and add. Does not delete code/anything that was typed into the file last.  


---
## Collaberation
**Clone**  
Cloning allows you to make multiple copies of one repository.
1. Go into Github and go to the repository you want to clone
2. Click the green `clone or download` button and make sure befor copying the link it says: Clone with **SSH**
3. Go to Cloud 9 and into the directory you want the repo to go in
4. Type `git clone url` (`url` = ssh)
5. Once done `cd` into it

**Fork**  
Forking is to make a remote of someone elses repo and then clone it onto your local.  
You can't clone someone elses repo and push it without their permission. 
1. Go into Github and go to the repository you want to clone
2. At the top right corner there should be a button that says: `Fork` , click it
3. Once forked, next to the repo name it should say your username
4. Yor can now clone it into your directory

**Pull Request**  
Pull requests are when you clone someone elses repo and make changes to it then you add and commit, then in Github you summit the request.
