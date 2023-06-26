# **Intro_to_opensource_and_git_6**

<details id=1>
<summary><h2>Introduction</h2></summary>

In this tutorial you will learn how to access Git through the terminal. 

This tutorial is part of a larger series of tutorials created to teach J&J statistical programmers how to use open source, GitHub, and RStudio together.

</details>

<details id=2>
<summary><h2>Git bash</h2></summary>

We are now going to go through the basics of accessing GitHub through a terminal. Normally you should not need to do this. But on occasion it is handy if for some reason you have a software problem. You do not need to worry about remembering the commands. If you just remember that you can access through the terminal, and that a reference will give you the commands then you will be good!

1. Open the windows start menu and click all apps. 
2. Scroll down until you see the Git folder. 
3. Open the dropdown menu and select Git bash. 
4. A little window should open in the middle of your screen. 
5. First copy and paste the following command:
pwd
6. This tells to what directory you are in. 
7. Let's switch directories, type: 
cd Documents/github/<your test repo>
8. Great. Let's go back to File Explorer. Open the repo, and select New -> Text Document. 
9. In the first line type, "this is a test document"
10. Save the doc as test2.txt, and close it. 
11. Go back to Git bash. 
12. type the following commands, hit <enter> after each line  
git add *  
git commit -m "add text file"  
git push origin main
13. Let's wait 30s, go back to GitHub, and open your file. 
14. See that your changes are there? Now let's edit the file in GitHub. Add a new line that says, "This is a test line from GitHub"
15. Hit Commit. 
16. Go back to Git bash. 
17. Type:  
git pull
18. Go back to File Explorer, open your file, and verify that your edits are present. 
19. Well done!

</details>

<details id=3>
<summary><h2>Git from Rstudio</h2></summary>

** This needs to be updated

You can also access the terminal from RStudio. 
1. Open RStudio in SPACE. 
2. 
2. In the bottom right window of your screen, select Files, navigate to the opensource_sandbox repo folder, and open the Readme file. 
4. Add a line to it, "Update Readme for testing terminal"
5. Hit save
6. In the bottom left quadrant of your screen, select the "Terminal" tab. 
7. In the terminal type: cd GitHub/<your repo>
8. Hit enter. 
9. As before, enter the following lines and hit <enter> after each
git add *
git commit -m "test terminal"
git push origin main
10. Go back into GitHub and check your work. 
11. Nice job!!

</details>

<details id=4>
<summary><h2>Branches</h2></summary>

1. Go back to Git bash
2. Type:
git branch
3. You should get:
*main
4. Remember that you have a test branch? Not type:
git checkout test_branch
5. Go back to File Explorer
6. Create a new text file, add a line, and save it. 
7. Now come back to Git bash. 
8. Now type the following:
git add *
git commit -m "test terminal"
git push origin <test branch name>
9. Go back to GitHub in your browser, navigate to your repo, then the test branch, and verify that your file is present. 
10. Well done!

<details id=4>
<summary><h2>Notes and resources</h2></summary>

### Some notes on the terminal
There is no need to try and commit terminal commands to memory. Unless you really prefer commandline operations, remembering commands and navigating through workflows can be really hard. 

https://confluence.jnj.com/display/AGFR/DRUPAL+and+CANVAS+Training?preview=%2F358606675%2F381474906%2FSWTM-2088_Atlassian-Git-Cheatsheet.pdf



