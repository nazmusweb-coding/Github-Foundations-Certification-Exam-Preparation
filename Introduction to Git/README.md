# Git Command Summary from "Introduction to Git Recap"  

## User Configuration  
1. **`git config --global user.name "Your Name"`**  
   - **Purpose**: Sets the Git username for commits globally on the system.  

2. **`git config --global user.email "your.email@example.com"`**  
   - **Purpose**: Sets the Git email for commits globally on the system.  

3. **`git config --list`**  
   - **Purpose**: Displays the current Git configuration, including user information and other settings.  

---  

## Creating a New Repository  
4. **`mkdir cats`**  
   - **Purpose**: Creates a new directory named "cats".  

5. **`cd cats`**  
   - **Purpose**: Changes the current working directory to "cats".  

6. **`git init`**  
   - **Purpose**: Initializes an empty Git repository in the current directory.  

---  

## Tracking Files  
7. **`touch index.html`**  
   - **Purpose**: Creates an empty file named "index.html".  

8. **`git status`**  
   - **Purpose**: Displays the status of the repository, showing tracked and untracked files.  

9. **`git add .`**  
   - **Purpose**: Stages all changes (including new files) to be included in the next commit.  

10. **`git commit -m "Create an empty index.html file"`**  
    - **Purpose**: Commits the staged changes with a message describing the change.  

---  

## Modifying Files  
11. **`code index.html`**  
    - **Purpose**: Opens the "index.html" file in Visual Studio Code for editing.  

12. **`git commit -am "Add a heading to index.html"`**  
    - **Purpose**: Automatically stages and commits all tracked changes with a specified message.  

13. **`git log --oneline`**  
    - **Purpose**: Displays the commit history in a concise format.  

14. **`git diff`**  
    - **Purpose**: Shows the differences between the working directory and the last commit for unstaged changes.  

15. **`git commit -m "Add HTML boilerplate to index.html"`**  
    - **Purpose**: Commits the specified changes with a description.  

---  

## Managing .gitignore  
16. **`touch .gitignore`**  
    - **Purpose**: Creates a .gitignore file to specify files or directories Git should ignore.  

17. **`git add .gitignore`**  
    - **Purpose**: Stages the .gitignore file for committing.  

18. **`git commit -am "Make small wording changes; ignore editor backup files"`**  
    - **Purpose**: Commits all staged changes along with the .gitignore file.  

---  

## Adding New Files  
19. **`mkdir CSS`**  
    - **Purpose**: Creates a new directory named "CSS".  

20. **`touch CSS/.git-keep`**  
    - **Purpose**: Creates a .git-keep file to ensure the CSS directory is tracked in Git.  

21. **`git add CSS`**  
    - **Purpose**: Stages the CSS directory for committing.  

22. **`git commit -am "Add a simple stylesheet"`**  
    - **Purpose**: Commits all staged changes, including the CSS directory.  

---  

## Removing and Recovering Files  
23. **`git rm index.html`**  
    - **Purpose**: Removes the "index.html" file from both the working directory and staging area, preparing it for commit.  

24. **`git commit -m "Remove index.html"`**  
    - **Purpose**: Commits the deletion of "index.html" to the repository.  

25. **`git reset HEAD index.html`**  
    - **Purpose**: Unstages "index.html" from the staging area, retaining local modifications to the file without deleting it.  

26. **`git checkout -- index.html`**  
    - **Purpose**: Restores "index.html" to the last committed state, discarding any uncommitted local changes.  

---  

## Reverting Changes  
27. **`git commit -am "Adding incorrect content to index.html - BIG MISTAKE"`**  
    - **Purpose**: Commits changes that mistakenly included undesired content in "index.html".  

28. **`git revert --no-edit HEAD`**  
    - **Purpose**: Creates a new commit that reverts the changes made in the last commit without editing the commit message.  

---  

## Amending Commits  
29. **`git commit --amend --no-edit`**  
    - **Purpose**: Modifies the last commit without changing its commit message, allowing you to fix small mistakes (like typos) in the committed files.  

---  

## Checking Out Specific Commits  
30. **`git checkout <commit-hash>`**  
    - **Purpose**: Checks out a specific commit using its hash, allowing you to view the repository at that point in time.  

31. **`git checkout <commit-hash> .`**  
    - **Purpose**: Checks out all files from a specific commit hash, restoring the repository to that state.  

---  

## Finalizing Changes  
32. **`git commit -m "Reverting back to correct content in index.html"`**  
    - **Purpose**: Commits the changes made to revert to the previous correct state of "index.html".  

33. **`git log --oneline`**  
    - **Purpose**: Displays the updated commit history after making changes.  

---  

## Summary  
This summary provides an overview of the key Git commands covered in the video, offering clear distinctions regarding file management, staging, and recovery operations.