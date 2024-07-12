DevOps Lab

Exercise 1

  Exploring Git Commands through Collaborative Coding – Basic Git


1.  Open your terminal (Command Prompt, Git Bash, etc.).

2.  Navigate to the directory where you want to create the repository.

3.  Initialize a new Git repository by running the following command:

    *git init Master*

4.  Change directory into the new repository:

    *cd Master*
     
    ![Screenshot from 2024-07-12 13-44-40](https://github.com/user-attachments/assets/870fed3a-2fd0-46a7-ac36-4a7cbde8e455)


**Create a new text file named ReadMe.txt using any text editor**

1.  Add the new file to the staging area:

    *git add ReadMe.odt*

2.  Commit the change with a message:

    *git commit -m "Add ReadMe.odt"*

![Screenshot from 2024-07-12 13-53-20](https://github.com/user-attachments/assets/8dd65f03-4e65-4915-bc60-3e0414cddbe8)


##### c. Exploring history

**Modify/add content to the text file**

1.  Stage the changes:

    *git add ReadMe.odt*

2.  Commit the changes:

    *git commit -m "Updated ReadMe.odt"*

![Screenshot from 2024-07-12 13-55-35](https://github.com/user-attachments/assets/3fdd8053-a709-4bb1-b8ca-aa9617a35466)


##### d. Branching and merging

**Create a new branch named "Updated_ReadMe" and commit the changes in
the branch**

1.  Create a new branch:

    *git checkout -b Updated_ReadMe*

2.  Open *ReadMe.odt* and make further modifications.

3.  Save the file and close the editor.

4.  Stage and commit the changes:

    *git add ReadMe.odt*

    *git commit -m "Updated ReadMe.txt in Updated_ReadMe branch"*

**Merge the changes from the Updated_ReadMe branch into the Master
branch**

1.  Switch back to the *master* branch:

    *git checkout master*

2.  Merge the changes from *Updated_ReadMe*:

    *git merge Updated_ReadMe*

  ![Screenshot from 2024-07-12 14-09-19](https://github.com/user-attachments/assets/b5971674-1a72-4f84-bdb7-140749f07a0d)


##### e. Collaborating with Remote Repositories

**Link your local repository to the remote repository**

1.  Create a repository on a hosting service like GitHub (if you haven't
    already).
2.  Copy the repository URL
3.  Link your local repository to the remote repository:

##### f. Push Changes

**Push your local commits to the remote repository**

1.  Push the changes to the remote repository:

    *git push -u origin master*

### Exercise 2: Implement GitHub Operations using Git

#### a. Cloning a Repository

**Clone the repository of your project from GitHub**

1.  Copy the URL of the repository you want to clone
    https://github.com/nithyapandurangan/ElevateHome

2.  Clone the repository:

    *git clone https://github.com/nithyapandurangan/ElevateHome.git*

3.  Change directory into the cloned repository:

#### b. Making Changes and Creating a Branch

**Navigate into the cloned repository, do the necessary changes and
check the status of the repository**

1.  Open *ReadMe.md* and make any necessary changes.

2.  Save the file and close the editor.

3.  Check the status of the repository:

    *git status*

4.  Create a new branch:

    *git checkout -b feature-update*

#### c. Pushing Changes to GitHub

**Add Repository URL in a variable**

1.  Add the remote repository URL in a variable:

    *REPO_URL="https://github.com/nithyapandurangan/ElevateHome.git"*

2.  Stage and commit your changes:

    *git add ReadMe.txt*

    *git commit -m "Update ReadMe.txt in feature-update branch"*

**Push the local branch to the repository**

1.  Push the changes to the remote repository:

    *git push -u origin feature-update*

#### d. Collaborating through Pull Requests

**Create a pull request on GitHub**

1.  Go to your repository on GitHub.
2.  Click on the "Pull requests" tab.
3.  Click on "New pull request".
4.  Choose the base branch (e.g., *master*) and compare it with the
    branch you want to merge (e.g., *feature-update*).
5.  Review the changes and click on "Create pull request".
6.  Add a title and description for the pull request.
7.  Assign reviewers if necessary.

**Reviewers approve the pull request, merge it into the base branch**

1.  Once reviewers approve the pull request, click on "Merge pull
    request".
2.  Confirm the merge.

#### e. Syncing Changes

**After the pull request is merged, update your local repository**

1.  Update your local repository with the latest changes from the remote
    repository:

    *git checkout master*

    *git pull origin master*

