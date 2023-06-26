# **Intro_to_opensource_and_git_4**

<details id=1>
<summary><h2>Introduction</h2></summary>

In this tutorial you will learn how to use a Git client, or an application on your local PC (or Mac) that interacts with Git. This will allow you to create, open, and edit files locally, and then upload them to GitHub.  

This tutorial is part of a larger series of tutorials created to teach J&J statistical programmers how to use open source, GitHub, and RStudio together.

</details>

<details id=2>
<summary><h2>Git clients</h2></summary>

### What is a Git client?
* So far we have been using a web based platform called Github. 
* As a reminder, GitHub hosts Git in the cloud, and provides a web-based interface  to access our Git repositories. 
* But maybe we are developing and testing our code locally with a platform such as with R or Python. In this case we likely want to also be able to store and access our code locally.
* In this case we will need a Git client installed on our local machine that will facilitate this process. 
* Some examples of Git clients are GitHub desktop and Sourcetree. RStudio also has features that let us use it as a client.

</details>

<details id=3>
<summary><h2>What is a clone?</h2></summary>
### What is a clone?
* A clone is a copy of a repository that we are going to create on your local machine. 
* When you edit documents in your repository you will go through a series of steps to align your remote version with the primary branch, which we will call origin. 
* You will learn how to make those steps with SourceTree. 
* There are a number of different Git clients that one can choose to use. You can also use the commandline for Git commands. The software you use may make these steps look a bit different, but the concept is always the same. 

</details>

<details id=4>
<summary><h2>Sourcetree intro & setup</h2></summary>

Sourcetree is one of the applications we can use to access Git. Let's go through the steps of setting this up. 

* Let's start by getting the application if you do not have it already. Sourcetree is available as approved software through J&J. To install it, follow these steps:
1. Step one
2. Step two

* Alternatively, you may got here: [Sourcetree](https://www.sourcetreeapp.com/) to install the software. 

### Sourcetree setup. 
1. Open Sourcetree
2. When asked what BitBucket source you use select BitBucket server
![Image of buckets](https://confluence.atlassian.com/get-started-with-sourcetree/files/847359094/946039150/1/1519833910087/sourcetree_account.png)

3. You will be asked for your login info, please add it
4. Go to Tools -> Options -> Authentication
![menu](https://confluence.jnj.com/download/attachments/137075777/step%201.png?version=1&modificationDate=1548762406000&api=v2)
5. Select "Add"
6. Change the Hosting service to GitHub
7. Preferred protocol should be "HTTPS"
8. Leave authenticiation as OAuth. 
[creds dialog box](https://confluence.jnj.com/download/attachments/137075777/step%204.png?version=1&modificationDate=1548763291000&api=v2)
9. Enter your user name
10. Hit Refresh OAuth token. 
11. You will be prompted to login and authorize SourceTree. Please authorize. 

Sourcetree resources:
https://confluence.atlassian.com/get-started-with-sourcetree

### Make a video for intro to using Sourcetree

### Find a good how to doc for Sourcetree
I don't like reinventing the wheel here. But Sourcetree has updated their software and their knowledge docs pre-date the software updates. J&J docs also seem somewhat outdated. 

</details>

<details id=5>
<summary><h2>Set up Git folder</h2></summary>

I like to set up a folder to house all of my Git repositories. It allows me to differentiate between Git and non-Git folders. 

1. Open File Explorer
2. Navigate to "C:/Users/<your name>/Documents"
3. Create a new folder called git_repos
4. In SourceTree, go to Tools -> Options
5. Scroll down to Repo settings
6. In "Project Folder", add the path of the git_repos folder: "C:/Users/<your name>/Documents/git_repos"
7. Hit "OK"

</details>

<details id=6>
<summary><h2>Sourcetree clone a repo</h2></summary>

### Cloning a repository
Now that we have set up our account, we can clone one of our Git repositories onto our local machine. Let's do that..

1. Add a tab (plus sign) to your SourceTree browser. 
2. Select "Clone"
3. In the next window, see the note that says, "Cloning is even easier if you set up a remote account"
4. "Remote account" is an active link, press it. 
5. If we set up your account with SourceTree correctly, all of your Git repositories will already be linked. 
6. In the "Remote repositories" window, select your GitHub account, and a list of your repositories should populate on the right of your screen. 
7. Select your test repository, and click the link "Clone" to the right of your repo name. 
8. SourceTree should autofill all of the fields, ensure that the second box containing the path of your repo looks something like this, "C:/Users/<your name>/Documents/git_repos/test_repo." Including "git_repos" in the path will keep your repository isolated from the rest of your documents. 
9. Now open the File Explorer (or finder) on your computer and verify that a folder with your repo name is now there. 
10. Good job!

</details>


 <details id=8>
<summary><h2>Test SourceTree with test repo</h2></summary>
OK, we've cloned a repo, now let's learn how to make it work with Git.

### Commit and push

1. Navigate to your test repo (the one you just cloned) in File Explorer
2. In File Explorer select "New" -> "Text Document"
3. Name the document "Testdoc.txt"
4. Open the text doc and add a line like, "This is a test document"
5. Save it, and close it.
6. Go to SourceTree.
7. In the bottom left of your window find the section labelled "Unstaged files" and select your test doc. 
8. Select the "Stage selected" button to the right
9. Select "Commit" in the top left of the screen
10. A new screen appears. We need to make a note for our commit. Making it unique will allow us to find this update at a later point in time should we need to. 
11. Find your user ID at the bottom of the screen, and note the dialog box below, Add your note here. Something like, "Create test_doc"
12. At the far bottom right, select "Commit"
13. Almost there.. Back at the top left, find the button labelled "Push." There should be a little 1 next to it indicating that there is 1 Commit to push. Press the "Push" button. 
14. In the next window, make sure your paths look correct, and hit "Push" again. 
15. Done! You have now staged, made a commit, and made a push!

### Fetch and pull

8. The file should appear in the window in the upper left
* Commit
* Push
* Wait 30s, then let's go back to your account in GitHub online, and let's take a look. Your file should be there. 
* Go ahead and open the file. Let's edit the first line. 
* Type something like, "This is an update to the test file"
* Add a comment like, "Update test file"
* Hit "Commit"
* Now, go to GitHub desktop and select "Fetch" and then "Pull"
* Open the test doc and verify that your file and its changes are present.


</details>

### This tutorial will guide you through the use of a client to access Git. 
* Remember that GitHub is a platform that we use to access Git. 
* Git is the tool that's under the hood and is allowing us to share. 
* We have other tools that we can use to access Git including:
** Sourcetree
** RStudio
** Git via the command line
*** Git runs off Linux. If you happen to have a Mac, you can install Git and run it from the terminal. If you are using a PC, you need to install another application to access Git via the "Commandline."

### Let's DO teach people how to use GitHub desktop if possible. It's simple and straightforward. 

## Let's first create a directory to hold all of our repositories. 
* Open File Explorer on your PC
* Go to C:\Users<your_name>\Documents and create a folder to hold your repositories. Let's call it "Git_repos"

* Go here [Install GitHub Desktop](add link here)
* Go to your GitHub account page and pick a repository
* Hit "Code" and select the entire webpage
* Go back to GitHub desktop
* Select Clone
* Add the webpage



## Note that this gives you a few options. You can create and edit documents via GitHub, and now that you have cloned your repository you can also do so via GitHub desktop. 

* This means that you can create and edit a document on your computer, and then save it to GitHub. 

## OK. This gets us through the basics:
1. Logging on
2. Creating repo
3. Editing readme
4. Creating a branch
5. Pull request
6. Merge the pull request


## Great work! Let's do this now with an application called SourceTree. This is an approved app for J&J, so it is worth learning how to use it. 

* Go here [Install SourceTree](add link here)
* Go to your GitHub account page and pick a repository that has not yet been cloned to your computer. 
* On the menu, go to "File" -> "Clone/New" 
* Add the URL to the first box
* Add your repo to the second box, make sure you add it to the "Git_repos" directory. It should look something like:
"C:\Users\Josh Lynch\Documents\git_repos\my repo here"
* Add the name of your repo to the "Name" box
* Hit "Clone"





* Go back to GitHub desktop
* Select Clone
* Add the webpage

* https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud


