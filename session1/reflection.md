Q1 Why is a commit history useful when maintaining software? Give one concrete maintenance

situation (for example finding when a bug appeared) and refer to your own commits.



* Having a commit history gives the user a chronological record of changes made, when, and why they occurred. For example, if a secret or unwanted log file is accidentally tracked later during maintenance, checking past commits helps identify when the behaviour was introduced. In my 'scm-lab-evidence', commits such as "Add. gitignore" and "Add Session 1 notes" show how updates were made step-by-step. Also, the simple, short commit messages make it easy to pinpoint issues instead of needing to go through the whole project folders and files 1 by 1.





Q2 Explain the difference between Git and GitHub, using your two repositories (the exercise

repository and scm-lab-evidence) as examples.



* Git is the distributed version control tool installed in my computer that tracks snapshots, branches, and local history. GitHub is a web-based platform that hosts remote repositories and supports collaboration, pull requests, and exercise workflow. My GitHub Skills exercise repository uses GitHub guided repository and pull request workflow to practice collaboration features. Meanwhile, 'scm-lab-evidence' started locally with Git, then linked to GitHub for me to push commits and test cloning and pulling.



Q3 In the GitHub Skills exercise you worked on a branch and used a pull request instead of changing

main directly. What risk does this reduce?



* It reduces the risk of breaking the main codebase with half-finished or buggy changes. Because 'main' stays isolated until changes are reviewed and merged, other work or releases are less likely to be disrupted. Pull requests also create a clear checkpoint to inspect diffs and verify that everything looks right before integration. Overall, branching is a safer habit than editing 'main' directly.





Q4  State which of your commands changed only your computer and which changed GitHub.



* The commands that changed my computer are such as "git init", "git add", "git commit", "git switch", "git merge", "git branch-d", and "git restore". These changed my local repository and working directory on my laptop.
* Running "git pull" fetched remote changes from GitHub and updated my local repository and working tree. "Git clone" copied a repository from GitHub to my machine, and "git push" sent my local commit up to update the repository on GitHub.



\-----------Part 1. Learn the Concepts------------

Without looking back at the videos, fill in your own definitions in the table below (on paper or in a text

file). You will compare them with the answer key in Appendix A, then use them in your reflection.



\-----OWN DEFINITION-----

1. Repository: It is the project folder that contains recorded history and changes
2. Working tree (working directory): It is the general project that user is working on
3. Staging Area (index): The area that stores all information before pressing commit
4. Commit: The action of taking the information from staging area to directory
5. Branch: It separates a portion of the project from the main so that users can work on it separately without disturbing the main.
6. Merge: To combine the separated branches
7. Remote: A copy of a repository
8. Push: To upload a commit
9. Pull: To download a commit and combine it into the project
10. Clone: To copy a repository



\-----FIXED DEFINITION FROM PRACTICAL 1 PDF + NEW KNOWLEDGE I UNDERSTOOD-----

1. Repository: The complete project directory along with its entire recorded version history and metadata (stored inside the hidden .git folder).
2. Working tree (working directory): The actual project files and folders currently checked out on your computer that you actively view, edit, and create.
3. Staging Area (index): An intermediate preparation zone that holds the specific list of file changes you have selected (via git add) to include in your next commit.
4. Commit: A permanent, saved snapshot of the staged project state in the repository's history, recorded with a descriptive message, author identity, timestamp, and unique ID.
5. Branch: A lightweight, movable pointer to a specific line of commits that allows you to develop features or fixes in parallel without affecting the main codebase.
6. Merge: The operation of combining the commit history and file changes from one branch into another (such as integrating a feature branch back into main).
7. Remote: A version of your repository hosted on another server or network location (such as "origin" on GitHub) used for backup and team collaboration.
8. Push: The action of uploading your local committed snapshots from a local branch to a remote repository so others can access them.
9. Pull: The action of fetching new commits from a remote repository and immediately integrating (merging) them into your current local branch and working tree.
10. Clone: The action of downloading a full copy of an existing remote repository—including all its files, branches, and complete commit history—onto your local machine for the first time.



