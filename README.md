# GitHub Tutorial

_by Riley K_

---
## Git vs. GitHub
Git is the tool that you use inorder to in  Github, which is the platform where you do can store your projectsyou make. 
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
1. Start off by creating a Github account with your email (username: `<your name>`, if you are a HSTAT student use your HSTAT email but without the `@hstat.org`)
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
10. Go to Github, at top-right click the `+`, create a new repository, name it and then click `create repository` 
11. Once created, make sure the url is under SSH, then go to the second section to copy and paste the following lines on to your Cloud 9(one at a time)  

**Congrates! You're finally done setting up your Github and Cloud 9 account!**


---
## Repository Setup



---
## Workflow & Commands



---
## Rolling Back Changes