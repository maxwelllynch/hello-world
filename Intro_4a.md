# **Intro_to_opensource_and_git_4**

<details id=1>
<summary><h2>Introduction</h2></summary>

In this tutorial you will learn how to access GitHub through RStudio. 

This tutorial is part of a larger series of tutorials created to teach J&J statistical programmers how to use open source, GitHub, and RStudio together.

</details>

<details id=2>
<summary><h2>Git clients</h2></summary>

### What is a Git client?
* So far we have been using a web based platform called GitHub. 
* As a reminder, GitHub hosts Git repositories in the cloud, and provides a web-based interface to access them. 
* But maybe we are developing and testing our code locally with a platform such as with R or Python. In this case we likely want to also be able to store and access our code locally.
* In this case we will need a Git client installed on our local machine that will facilitate this process. 
* Some examples of Git clients are GitHub desktop and Sourcetree. RStudio also has features that let us use it as a client.
* We are going to learn how to use RStudio as a Git client.

</details>

<details id=3>
<summary><h2>Install Git</h2></summary>

### Install Git

* Open your apps and verify that Git is not installed on your machine. 
Follow these instructions to install Git. These can also be found [here](https://confluence.jnj.com/display/ABES/GIT+Guides+and+Tips#GITGuidesandTips-3.InstallGit)

1. Open J&J [app store](https://jnjitod.service-now.com/appstore) and search for "git":
![J&J storefront](https://confluence.jnj.com/download/attachments/319395571/image2019-11-19_15-33-3.png?version=1&modificationDate=1633033542413&api=v2)
2. Select the most recent version of "The Git Development Community GIT" and then click add. On the following screen, click add again to have the app added to your cart:
![cart](https://confluence.jnj.com/download/attachments/319395571/image2019-11-19_15-34-5.png?version=1&modificationDate=1633033542381&api=v2)
3. Click on My Cart
4. Click Install on this machine to have Git app installed. 

</details>

<details id=4>
<summary><h2>RStudio</h2></summary>

### RStudio
* Please follow these steps to have an official version of RStudio installed on your computer. 
1. Open J&J app store and search for "RStudio".
2. Select the most recent version of "RStudio Desktop" and then click add. On the following screen, click add again to have the app added to your cart:
3. Click on My Cart
4. Click Install on this machine to have RStudio installed. 

</details>

<details id=5>
<summary><h2>Install R</h2></summary>

* Install R
1. Open Crome and go to the [R website](https://www.r-project.org/)
2. At the top under "Getting Started," click "download R" in blue. 
3. In the next screen select your mirror. Try "https://cloud.r-project.org/" at the top. 
4. In the next screen Select "Download R for Windows." It should be the third bullit down in the first section of the page. 
5. In the next screen click the blue highlighted link "install R for the first time"
6. At the top of the next page, select the blue highlighted link "Download R-(version) for Windows"
7. A downloaded file should appear in the bottom left of your Chrome browser. If it is not there then look in your "Downloads" folder. Open the file. 
8. Install R using default options. 

</details>

<details id=6>
<summary><h2>Configure git</h2></summary>

* Open RStudio, and go to the terminal
* Enter the following commands, substituting your info in as needed, remove the <>:
git config --global user.name '<Jane Doe>'  
git config --global user.email '<jane@example.com>'  
git config --global --list  
git config --global init.defaultBranch main

* You will also need to generate and authorization token within GitHub. Go [here](https://github.com/settings/tokens) and generate a token. 
* Select "repo"", "user", and "workflow".
* Copy the generated token to your clipboard and save it. 
* You will use this token in the future when asked for your password. 
* You can read more on authorization tokens [here](https://happygitwithr.com/https-pat.html)

* Set up a GitHub folder:
1. Open File Explorer
2. Go to "Documents"
3. Create a new folder called "GitHub"
We will use this folder to house GitHub repos, this will keep them differentiated from non-Git folder on your computer. 

</details>

<details id=5>
<summary><h2>RStudio and GitHub</h2></summary>

### Clone a repository

We are going to loosely follow the directions [here](https://happygitwithr.com/push-pull-github.html)
I've created a copy of them here for your convenience. 

1. Go to https://github.com and make sure you are logged in.
2. Go to repositories and select your test repo
3. Now click the big green button that says “<> Code”.
4. Copy a clone URL to your clipboard. Copy the HTTPS URL.

### Pause

What is a clone?
* A clone is a copy of a repository that we are going to create on your local machine. 
Wait a minute. Didn't you say that a branch is a copy of a repository? 
* Yes. They are both copies. A clone is a copy of a repository that we put in another location, such as our local computer. 
* When you clone a repo you are copying everything. Including the branches. 
* A branch is a copy of the repo used for development. 
* When a clone is created on a remote machine, we have to take extra steps to make sure that the versions stay synchronized. 
* You will edit the files in a cloned repo on your local machine, and then push them to GitHub. 
* Let's continue. 

We are going to follow the steps (here)[https://happygitwithr.com/new-github-first.html#new-github-first]
they are copied for convenience. 

1. In RStudio, start a new Project:File > New Project > Version Control > Git. 
2. In the "repository URL" paste the URL of your test repository (that you copied). It will be something like this https://github.com/jennybc/testrepo.git.
3. In the 3rd box down, navigate to "C:/Users/<Your name>/Documents/GitHub"
4. select "Open in new session".
5. Click "Create Project" to create a new directory, which will be all of these things:
* a directory or “folder” on your computer
* a Git repository, linked to a remote GitHub repository
* an RStudio Project

</details>

<details id=5>
<summary><h2>A quick look around</h2></summary>
OK. Let's take a look around. In the bottom right quadrant of RStudio, please select "Files" and navigate to your repo. Note that all of the files you created in GitHub are now copied and visible within your RStudio workspace. Not bad! Now we are going learn how to move back and forth between your local repo version and the version on GitHub. This is called committing and pushing, and fetching and pulling. 

</details>

<details id=6>
<summary><h2>Commit and push</h2></summary>
### Commit and push
We are going to edit your Readme file, and then push those changes onto GitHub

1. Go to RStudio, and see the list of files on the lower right quadrant of your screen. 
2. Open your Readme file. 
3. The Readme contents should now appear in the upper left quadrant of RStudio. 
4. Add a new line. Type, "testing RStudio"
5. Save it
6. Look at the menu bar in the upper right of RStudio. Click the "Git" tab. 
7. You should see a list of files including your Readme. Click the boxes to the left of the file names. Note that the column header says "Staged"
8. Now click the "Commit" button. A new window opens. 
9. Note the list of files and note the Commit window in the upper right. You will need to add a message, like "test RStudio"
10. Click the "Commit" button under the Commit window. 
11. Close the message box that appears when it is complete.
12. Now in the upper right of the active screen, press "Push", there is a green up arrow next to it. 
13. You can now close the message window and the Commit window. 

</details>

<details id=7>
<summary><h2>Pull</h2></summary>

### Pull

1. Wait 30s, then let's go back to your account in GitHub online, and let's take a look. Find your Readme file. 
2. Go ahead and open the file.
3. Note that your changes are there!
4. Let's update the file. Click edit and type something on the next line. Like "Tag you're it"
5. Hit "Commit changes"
6. Now, go to back to RStudio.
7. In the upper right again, click the "Pull" button next to the blue down arrow.
8. Close the message box again. 
9. Open your Readme again, or just look at it if you did not close. Note that your changes are now there. 

### Congrats!!

You have now learned how to clone, push, and pull via RStudio!! 


