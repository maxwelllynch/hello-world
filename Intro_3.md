# **Intro_to_opensource_and_git_3**

<details id=1>
<summary><h2>Introduction</h2></summary>

This tutorial will be pretty short. We are going to use a [GitHub skills](https://skills.github.com/) tutorial to run you through how to deal with merge conflicts, and how to update your branch from the main branch. 

This tutorial is part of a larger series of tutorials created to teach J&J statistical programmers how to use open source, GitHub, and RStudio together.

</details>

<details id=2>
<summary><h2>Merge Conflicts</h2></summary>

### Merge conflicts
* Sometimes we develop code in a branch off of main (or another branch that we branched off of), and an update is applied to the main branch while we are working.
* When we create a pull request there is now an issue. Which edits are we supposed to use?
* The following tutorial will guide you through this scenario: [Merge Conflicts](https://github.com/skills/resolve-merge-conflicts)

</details>

<details id=3>
<summary><h2>Merge main into branch</h2></summary>

### Merging back into a branch

Sometimes we may have a reason to merge our main branch back into the branch we've created. Reasons for this might be:

* Someone else is working on other files within the repository, and we want to update those.
* Someone else is working on another part of the same file, and we want to update it. 

Regardless of the reason, it is handy to be able to merge branches in all directions. Please follow the following steps to try this out. 

1. Open your test repository and navigate the the "Main" branch
2. Go to "Add file" -> "Create new file"
3. Name your file something like "test2.txt"
4. Type something in the first line, "This is a test file" will suffice. 
5. Scroll down and hit "Commit new file"
6. You should now be able to see your file in the list of repository files. 
7. Now select "Pull requests" from the main menu.
8. Select "New pull request"
9. A page labeled "Compare" should appear, and you should have 2 boxes with an arrow in between. The arrow should point **from** compare **to** base.
10. Note that there is a drop down menu for each branch. This means that you can choose to merge from and into any 2 branches you may choose. 
11. Select "Main" for your "Compare" box and "Test1" for the "Base" box. 
12. Select "Create pull request"
13. Add a title, like "Merge main"
14. Select "Create pull request," the "Confirm merge"
15. The next window should tell you that you have no conflicts with base. Select "Merge pull request"
16. Now click on your repository in the upper left. It will likely have taken you back to the "main" branch. Select your test branch from the drop down menu. 
17. Both of your files should now be in the test repository.
18. Nice work!


</details>


