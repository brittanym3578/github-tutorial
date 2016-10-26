# GitHub Tutorial

_by Brittany Misacango_

---
## Git vs. GitHub
Git and github are both brilliant ways to manage code that almost every developer uses it, but at the same time they have their differences. The main reason as to why they are different is because git is the version control tool that GitHub is built on top of 
and GitHub is a website where you can upload a copy of your Git repository. Their differences are listed below.

##### Differences  
* Git keeps snapshots of code
* Github is not needed in order to use Git but Git is required in order to use Github
* Github stores code in the cloud and it's easy to track changes 



---
## Initial Setup

**How to make a Github account**

1. Go to [github.com](github.com) and press the button that says "sign up"
   * Then enter the information that is required
     [image](https://snag.gy/DKamFX.jpg)
   * There will be two options for you which are "Unlimited public repositories for free" or "Unlimited private repositories for $7/month." Choose either one of your preference
   * once you're done signing up, check your email and verify with github
  
2.Go to c9.io
   * create an account(first/last name, email, password)
   * once set up, press on the gear in the top right corner
   * go to connected services
   * connect your github with cloud9 by clicking on the connect button
  
3.In the future you will sign into cloud9 using your github account
   * [if you want to sign-in to github using c9, this is what you should do.](https://raw.githubusercontent.com/OperationSpark/using-c9/master/img/c9-signin-github.png)  

**Follow these instructions below for how to use SSH**

1. First make sure you are in your github account.

2. Go to your settings which is located in the top-right profile icon 
3. Now that you're their, in the left side-bar you are going to see "SSH and GPG keys" (Click on that)
4. Press on New SSH key and put a title of your preference
5. Now for the _key_, which is below the title, switch to your cloud9 tab
6. Click on the gear icon which is on the top-right 
7. Press on SSH keys tab and copy/paste your SSH key into GitHub
8. Add the SSH
9. Lastly go to your cloud9 and open github-learning IDE


---
## Repository Setup

__**Down below are the instructions for how to create your 1st repository**__

1. go to Github.com and click on the **(+)**, then click **New Repository**
    * [here is an example of what it should look like](https://github-images.s3.amazonaws.com/enterprise/11.10.340/user/assets/images/help/repository/repo-create.png)

2. Create a short name for your repository

3. Make sure it's **Public**, so people can check out your work, fork it and add their own changes to make it better (with your permission)

4. Select **initialize this repository with a README.md**

5. finally, click **Create Repository** (remote repository)

6. Copy/paste the two links under the section titled "or push an existing repository from the commnad line, one at a time"
    * After creating the repository on cloud9, follow the steps below and then continue with these two links from above

**Add, Commit, and Push your First Changes**

_Make your first repository on cloud9:_

1. Go to c9.io and open your workspace

2. Start typing in the command line and make sure you're inside your workspace
  * ``` cd ~/workspace```
 
3. Then type in...
    * ``` mkdir and (the name of your first repository on github)```
    * Example: ```mkdir first-repo```
    
4. To go inside of your repository, type 
    * ``` cd (name of your repository)```
    
5. Then, type:
    * ``` git init```
 
_**Add a README.md file:**_

1. In your command line, after the code you you are typing you shoul put:
    * ``` touch README.md```
    
2. To go to the file you can either press on the file in the sidebar under the name of your repository or you can type ``` c9 README.md```

3. Now that you are in the README.md file, type in a message that will show up in your github

4. Make sure your work in the file is saved by pressing "command" & "s"

5. Then in the command line, type:
    * ``` git add .```

6. Next, make a commit message that is in the present tense, short, to the point, and about the change you just executed; type:
    * ```git commit -m "message " ```

7. Copy/paste the links one at a time in the command line after following the previous directions
    * ```git remote add origin git@github.com:brittany3578/third-repo.git ```
    * ``` git push -u origin master ```
    
---
## Workflow & Commands
Command        | Definition/Use
---------------| -------------
```git init```|Initializes git in the directory (repository); only done once when the folder is just created. If git is initialized in the wrong directory, then you technically would be working on your project in the wrong place and not the folder originally thought of so you have to do ```cd``` into the directory of your choice and then initialize git.
```git add .```|Adds the current/entire directory
``` git commit -m "message"```|Takes a snapshot of the files on the stage. It should describe what was modified in the snapshot
``` rm -rf .git```|Uninitializes git in the working directory. Rm means remove and the r means recursively, which makes it continue deleting until everything in that specific place is gone and the f means forcefully, which means that it will delete no matter how protected it is.
```git push -u origin master```|Pushes committed changes into the repository
```git log```|This shows the previous commands in detail. It is listed in reverse chronological order
```git diff ```|Will show you the differences between your current commit and the previous commit
```q```|Quits the git diff mode
```git status```|Optional command that lets you see files that have been edited since the last commit. It would either be red or green
```git add --all```|Includes all changes aswell as the deleted files

## Collaboration
#### Fork
Forking is a way to create a replica of someone else's remote repository so that you can take their project, make changes, and push those changes to the forked remote repository but without disrupting the original project. If you want to fork something you just have to go to that project and click "fork" on the top right corner. 
#### Pull Requests
Pull requests are ways that people who have forked your repository and have made changes to it can let you see those changes and possibly add them to the original project.
You click pull request to suggest those changes when you submit a pull request in your forked repository.
[image](https://snag.gy/mFtbLW.jpg)
### Cloning
It is making a copy from your remote repository (lives in the cloud) to your local repository
1. [image](https://snag.gy/Dq1E9j.jpg)

2. [image](https://snag.gy/Bz3a0L.jpg)

3. after cloned, cd into that directory 

### Pull requests: 
Help make other people’s projects better by offering your changes to them about the original project  
Step 1: [image](https://snag.gy/DYHlEg.jpg)  
Step 2: Add a description of what you want to change and submit your pull requests
[image](https://snag.gy/cDPvyM.jpg)