---
title: "Git-2 Interview Q/A"
datePublished: Sat Oct 14 2023 18:04:47 GMT+0000 (Coordinated Universal Time)
cuid: clnqckts4000b09ju3gkm53y9
slug: git-2-interview-qa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1700672740656/f6cbdd55-cad8-4552-b86e-d9cf43079d70.png
tags: github, devops, devops-articles, gitcommands, git-interview-questions-and-answers

---

1. **What is GIT?**  
    Git is an open-source distributed version control system that enables efficient and organized management of source code and project files. It provides a way to track changes, collaborate with multiple people, and maintain a history of project progress.
    
2. **Which language is used in Git?**  
    Git is primarily implemented in the 'C' programming language. This choice of language makes Git fast and efficient, reducing runtime overhead seen in higher-level languages.
    
3. **What is a repository in Git?**  
    In Git, a repository is a storage location where all Git files are kept, either locally on a developer's machine or remotely on a server. It is where Git stores all the metadata and history of a project.
    
4. **What is a 'bare repository' in Git?**  
    A "bare" repository in Git contains version control information but lacks working files or a working tree. It doesn't include the special .git sub-directory, and it is typically used on servers to share code. It consists of the contents of the .git sub-directory directly in the main directory.
    
5. **What is the purpose of the GIT stash?**  
    The `git stash` command in Git allows developers to save the current state of their working directory and index without committing changes. This is useful when you want to switch to a different task without losing your current work.
    
6. **What is GIT stash drop?**  
    The `git stash drop` command is used to remove or delete a specific stash item. You can either remove the last added stash item by default or specify the stash item you want to drop as an argument.
    
7. **What are the advantages of using GIT?**  
    Git offers several advantages, including data replication and replication, efficient network and disk performance, easy collaboration, the ability to work on multiple branches, and excellent source code management capabilities.
    
8. **What is the function of 'GIT PUSH' in Git?**  
    The `git push` the command is used to send local commits to a remote repository, updating the remote branches with your changes. It is essential for sharing your work with others and keeping remote repositories up-to-date.
    
9. **Why do we require branching in Git?**  
    Branching in Git allows developers to work on different features or tasks simultaneously without interfering with each other's work. It enables isolation, parallel development, and easy merging of changes into the main codebase.
    
10. **What is the purpose of 'git config'?**  
    The `git config` the command is used to configure Git settings at various levels (system, global, or repository-specific). It helps set preferences, user information, and repository behavior.
    
11. **What is the definition of "Index" or "Staging Area" in Git?**  
    The "Index" or "Staging Area" in Git is a crucial component that sits between your working directory and the repository. It's where you stage changes before committing them, allowing you to choose which changes to include in the next commit.
    
12. **What is a 'conflict' in Git?**  
    A "conflict" in Git occurs when the same part of a file has been modified differently in two different branches. When merging these branches, Git cannot automatically determine which change should take precedence, and manual intervention is required to resolve the conflict.
    
13. **What is the difference between** `git pull` **and** `git fetch`?  
    `git pull` fetches changes from a remote repository and automatically merges them into your local branch. `git fetch` also retrieves changes but does not perform an automatic merge. It stores fetched changes in a separate branch, allowing you to review and decide how to integrate them.
    
14. **How to resolve a conflict in Git?**  
    To resolve a conflict in Git, you need to edit the conflicting parts of the file, remove conflict markers, and then use `git add` it to stage the resolved file. After that, you can use `git commit` it to finalize the resolution.
    
15. **What is the purpose of the** `git clone` **command?**  
    The `git clone` command is used to create a copy of an existing Git repository, typically from a remote server. It allows you to start working on a project locally, with access to the entire version history.
    
16. **What does** `git pull origin` **do?**  
    `git pull origin` is a command that fetches all changes from the master branch in the remote repository named "origin" and integrates them into your current local branch. It effectively updates your local repository with changes from the remote.
    
17. **What does 'git commit' do?**  
    `git commit` is used to record changes to the repository. It creates a new commit with the changes you've staged, along with a commit message that describes what the changes are. It helps maintain a history of project progress.
    
18. **Why is GIT better than Subversion?**  
    Git and Subversion (SVN) are both version control systems, but Git is a distributed decentralized system, while SVN is centralized. Git is known for its speed, efficiency, and branching capabilities, making it more suitable for modern development workflows.
    
19. **Explain what a commit message is.**  
    A commit message in Git is a text description that accompanies a commit. It explains the purpose of the commit, the changes it introduces, and any relevant information. A well-written commit message is essential for understanding the history and context of a project.
    
20. **Why is it desirable to create an additional commit rather than amending an existing commit?**  
    Creating an additional commit instead of amending an existing one is preferred because it maintains a clear and accurate history of changes. Amending an existing commit can lead to confusion and the loss of previous states, making it harder to track the evolution of the codebase.
    
21. **What do 'hooks' comprise in Git?**  
    In Git, "hooks" are scripts or programs that can be executed before or after specific Git events, such as commits, pushes, or merges. Hooks allow developers to automate actions and enforce rules in the Git workflow.
    
22. **What is the distinction between Git and GitHub?**  
    Git is a distributed version control system, while GitHub is a web-based platform that provides Git repository hosting, collaborative development tools, and code management. Git is the software used for version control, while GitHub is a service that utilizes Git for code hosting and collaboration.
    
23. **In Git, how would you return a commit that has just been pushed and made public?**  
    To revert a commit that has been pushed and made public, you can either create a new commit that undoes the changes introduced by the problematic commit using `git revert`, or you can rewrite the project's history using `git reset` or `git push --force`, but this approach should be used with caution.
    
24. **What does the commit item contain in Git?**  
    A Git commit item contains a set of files representing the state of the project at a specific point in time, references to parent commit objects, and a SHA-1 hash that uniquely identifies the commit object.
    
25. **Describe the branching systems you have utilized.**  
    Different branching strategies can be employed in Git based on the project's needs. Some common branching systems include Feature Branching (isolating work on features), Task Branching (assigning tasks to specific branches), and Release Branching (creating branches for releases). The choice of strategy depends on the project and the organization's requirements.
    
26. **How will you know in Git if a branch has just been merged into a master?**  
    To check if a branch has been merged into the master branch, you can use commands like `git branch --merged` to list branches that have been merged into the current branch or `git branch --no-merged` to list branches that have not been merged.
    
27. **How would you fix a messed-up commit in Git?**  
    To fix a messed-up commit in Git, you can use the `git commit --amend` command to change the last commit's message or contents. It allows you to make corrections without creating a new commit.
    
28. **Mention the various Git repository hosting functions.**  
    There are several Git repository hosting services, including GitHub, GitLab, Bitbucket, SourceForge, and more. These platforms offer Git repository hosting, collaborative development tools, and code management services.
    
29. **Mention some of the best graphical Git clients for LINUX.**  
    Some of the best graphical Git clients for Linux include Git Cola, SmartGit, Git-g, Git GUI, Giggle, and qGit. These tools provide a user-friendly interface for managing Git repositories on Linux.
    
30. **What is Subgit? Why use it?**  
    Subgit is a tool designed for migrating from Subversion (SVN) to Git. It simplifies and streamlines the migration process, allowing organizations to transition from SVN to Git without changing their existing infrastructure. Subgit ensures a smooth and stress-free migration experience and provides the benefits of Git while retaining compatibility with SVN.