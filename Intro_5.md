# **Intro_to_opensource_and_git_5**

<details id=1>
<summary><h2>Introduction</h2></summary>

In this tutorial you will learn how to access Bitbucket through RStudio. 

This tutorial is part of a larger series of tutorials created to teach J&J statistical programmers how to use open source, GitHub, and RStudio together.

</details>

<details id=2>
<summary><h2>SPACE</h2></summary>

So far we have been accessing personal repositories in GitHub. J&J's programs are stored on another hosting service called Bitbucket.  
  
This brings up a big picture concept. This course is providing the tools for internal and external collaboration. J&J uses Bitbucket for its internal development. The platform will look a little different, but most of the concepts are the same. There are also likely to be different restrictions in place as you will be working in a regulated environment. 

Your R environment is also an important part of development within J&J. We are going to access RStudio through SPACE. 

This needs to be updated

1. Open chrome and navigate to [QA IDAR]add IDAR link here
2. Use your normal credentials to sign in. 
3. Start a new project. 
4. A version of RStdudio should now be open in your browser. 
</details>

<details id=3>
<summary><h2>RStudio</h2></summary>

Let's access and clone a repo in bitbucket through RStudio

1. Open a new tab and navigate to [Bitbucket]add bitbucket link here
2. Search for our test repo, "opensource_sandbox"
3. On the far left of your screen is a menu. If you hover over the first icon, it should say "Clone." Let's click that. 
4. Make sure HTTPS is selected and copy the URL.
4. Let's go back to RStudio. 
5. In the menu at the top let's go to Session -> New session
6. Now go to File -> New project -> Version control -> Git
7. Paste the URL (cntrl-V) in the first box
8. Hit Create Project
9. Once the project loads, look in the upper right and select Git. 
10. To the right on the menu bar, click the icon that contains 2 rectangles connected to a diamond. 
11. We are going to make a new branch, let's name it "testbranch_<your initials>"
12. Make sure that the "Remote" box says "Main." This is what we are branching off of. 
13. Make sure "sync with remote" is checked, and hit "Create branch." Name the branch "test_branch". Click "Create"
14. Now let's open the Readme again and add a line that says "test bitbucket"
25. Save your file. 
16. Repeat the steps outlined previously to push your change. The process is the same for bitbucket as it is for GitHub.

</details>

<details id=3>
<summary><h2>Bitbucket</h2></summary>

1. Go back to bitbucket and find the test repo again.
2. In the upper left, there is a drop down menu. It should say "Main"
3. Click the dropdown arrow and switch to your test branch
4. Click on the Readme file and note that your change is now there. 
5. Good job!

</details>

<details id=4>
<summary><h2>Bitbucket dev</h2></summary>

### Development in Bitbucket

As mentioned earlier, working in Bitbucket J&J will be a bit different as we have a very regulated work environment (this refers to access, software versioning, storage etc). You will likely see some changes in this environment compared to GitHub. It will be important that you do your work in a dev branch. You have already created a branch, so let's also add a file and set up a pull request. 

1. Open RStudio, and verify that you are working in your test branch. 
2. Now open RStudio and navigate to your test folder. 
3. Open the Readme, add a line that says "test pull request" Save the file. 
4. Commit, and push your changes. 
5. Good job, now go into Chrome and navigate to the test branch in bitbucket. Verify that your changes are present. 
6. Select your Readme file. Click the button labeled "Diff to previous." This shows what changed with your most recent commit. 
7. Now hover over the third icon down on the left menu. It should say "Create pull request." Click on it. 
8. The next screen should now show your 2 branches. The test branch should be labeled as "Source" and main should be labeled as "Destination." **Note that you can merge Main into a test branch by switching the branches.**  
9. Your title may already be filled in. If not, please add a title. 
10. Now add a description. "test pull request"
11. Note that there is a reviewers box. When developing software you would want to add a colleague to review your work. 
12. Select "Create"

</details>

https://confluence.jnj.com/display/ABES/GIT+Guides+and+Tips

