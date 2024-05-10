---
title: "GIT Interview Q/A"
datePublished: Sat Oct 14 2023 17:14:36 GMT+0000 (Coordinated Universal Time)
cuid: clnqasan6000c0al3bu9te22e
slug: git-interview-qa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1700673356606/2f208fd4-c3ea-4fa5-9edb-d24ad3ddb498.png
tags: github, git, devops, devops-interview-questions-and-answers, git-interview-questions-and-answers

---

1. What is GIT?  
    Git is an open-source distributed version control system and source code management (SCM) system with an insistence on controlling small and large projects with speed and efficiency.
    
2. Which language is used in Git?  
    Git uses the 'C' language. Git is quick, and the 'C' language makes this possible by decreasing the overhead of run times contained with high-level languages.
    
3. What is a repository in Git?  
    A repository consists of a list named .git, where Git holds all of its metadata for the catalog. The content of the .git file is private to Git.
    
4. What is a 'bare repository' in Git?  
    A "bare" repository in Git includes the version control information and no working files (no tree), and it doesn’t include the special .git sub-directory. Instead, it consists of all the contents of the .git sub-directory directly in the main directory itself, whereas the working list comprises of:
    
    * A .git subdirectory with all the Git-associated revision history of your repo.
        
    * A working tree, or find out copies of your project files.
        
5. What is the purpose of the GIT stash?  
    GIT stash takes the present state of the working file and index puts it on the stack for later and gives you back a clean working file. So, in case you are in the middle of an object and required to jump over to another task, and at the same time, you don't want to lose your current edits, you can use GIT stash.
    
6. What is GIT stash drop?  
    When you are done with the stashed element or want to delete it from the directory, run the 'git stash drop' command. It will delete the last added stash item by default, and it can also remove a specific stash if you include it as an argument.
    
7. What are the advantages of using GIT?  
    Some of the essential advantages of Git include data repetition and data replication, applicability, network performance, disk usage, ease of collaboration, and the ability to work on various projects within Git.
    
8. What is the function of 'GIT PUSH' in GIT?  
    'GIT PUSH' updates remote refs along with related objects.
    
9. Why do we require branching in GIT?  
    With branching, you can keep your branch and jump between different branches, allowing you to work on different tasks while keeping your recent work intact.
    
10. What is the purpose of 'git config'?  
    'Git config' is used to configure your preferences for the Git installation, describing repository behavior, preferences, and user information.
    
11. What is the definition of "Index" or "Staging Area" in GIT?  
    The "Index" or "Staging Area" is where you can make and review changes before committing them.
    
12. What is a 'conflict' in Git?  
    A 'conflict' occurs when the commit to be merged has changed in the same place as the current branch, making it difficult for Git to determine which change should take precedence.
    
13. What is the difference between git pull and git fetch?  
    Git pull updates the local branch with changes from a remote branch and merges them, while git fetch pulls the changes from a remote branch and saves them in a separate branch, requiring an additional merge step to update the local branch.
    
14. How to resolve a conflict in Git?  
    To resolve a conflict in Git, edit the conflicting changes, run 'git add' to stage the resolved changes, and then commit the merge.
    
15. What is the purpose of git clone?  
    Git clone generates a copy of an existing Git repository, making it the easiest way to obtain a copy of a central repository.
    
16. What is git pull origin?  
    'git pull origin' fetches commits from the source remote's master branch and merges them into the currently checked-out branch.
    
17. What does git commit do?  
    Git commit records changes to the repository, while git push updates remote references along with contained objects.
    
18. Why is GIT better than Subversion?  
    Git is preferred over Subversion because it allows version control, tracking code changes over time, and supports collaborative development, while Subversion lacks these capabilities.
    
19. What is a commit message?  
    A commit message in Git is a description of the changes made in a commit.
    
20. Why is it desirable to create an additional commit rather than amending an existing commit?  
    Creating an additional commit is preferred over amending an existing commit because it prevents the loss of the original commit's state and avoids unnecessary complications in the commit history.
    
21. What do 'hooks' consist of in Git?  
    Git hooks are shell scripts that are executed after running specific Git commands, such as post-commit scripts that run after a commit.
    
22. What is the distinction between Git and GitHub?  
    Git is a version control system, while GitHub is a web-based platform for hosting Git repositories and provides additional collaboration features.
    
23. In Git, how would you return a commit that has just been pushed and made open?  
    To return a commit that has been pushed and made public, you can either remove or fix the bad commit and push it to the remote repository, or you can create a new commit that fixes the changes introduced in the bad commit.
    
24. What does the commit item contain?  
    A Git commit contains a set of files representing the state of a project at a given point in time, references to parent commit objects, and an SHA-1 hash uniquely identifying the commit.
    
25. Describe the branching systems you have utilized.  
    Describe how you have used branching in previous projects, including feature branching, task branching, and release branching, and explain the purpose and benefits of each.
    
26. How will you know in Git if a branch has just been combined into a master?  
    You can use 'git branch -merged' to list branches that have been merged into the current branch and 'git branch -no merged' to list branches that have not been merged.
    
27. How might you fix a messed-up commit?  
    To fix a messed up commit, you can use the 'git commit --amend' command to edit the commit message.
    
28. Mention the various Git repository hosting functions.
    
    Various Git repository hosting functions include GitHub, GitEnterprise, [SourceForge.net](http://SourceForge.net), Visual Studio Online, and Pikacode.
    
29. Mention some of the best graphical Git clients for LINUX.  
    Some of the best graphical Git clients for LINUX include Git Cola, SmartGit, Git-g, Git GUI, Giggle, and qGit.
    
30. What is Subgit? Why use it?  
    Subgit is a tool for migrating SVN to Git, providing a stable and straightforward migration process without the need to change existing infrastructure. It allows utilizing all Git and Subversion features and offers a stress-free migration experience.