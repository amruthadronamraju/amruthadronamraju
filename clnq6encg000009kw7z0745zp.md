---
title: "Linux Interview  Q/A"
datePublished: Sat Oct 14 2023 15:12:01 GMT+0000 (Coordinated Universal Time)
cuid: clnq6encg000009kw7z0745zp
slug: linux-interview-qa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1700674810043/280c4e5e-67f4-4836-8636-9f4c19c13608.png
tags: linux, devops, linux-for-beginners, linux-basics, linux-interview-questions-and-answers

---

1. What is Linux?  
    Linux is an operating system based on the Linux Kernel, and it is known for being open-source, meaning its source code is freely available to users. Linux can run on various hardware platforms and provides a cost-effective alternative to commercial operating systems. Users can easily modify and customize the source code to create variations tailored to their needs.
    
2. Who invented Linux?  
    Explain the history of Linux. Linux was created by Linus Torvalds, a student at the University of Helsinki in Finland, in 1991. Linus initially developed Linux as a way to obtain a free academic version of Unix. Over time, Linux gained popularity and evolved into a full-fledged operating system, with contributions from a global community of developers.
    
3. What is a Linux Kernel?  
    The Linux Kernel is the core component of the Linux operating system. It serves as an intermediary between software applications and the computer's hardware. When software applications need to interact with hardware components, the kernel facilitates this communication. For instance, if you want to play a song, your media player requests the kernel to access hardware resources like speakers or headphones. Linux Kernel is released under the General Public License and is open for modification.
    
4. What is Shell?  
    A Shell is a computer program that acts as an interface between users and the Linux Kernel. Users interact with the shell by issuing commands, writing scripts, or running programs. The shell interprets these human-readable commands and converts them into instructions that the kernel can understand and execute.
    
5. How many types of Shells are there in Linux?  
    There are five main types of shells in Linux: a. C Shell (csh): Known for its C-like syntax and features such as spelling checking and job control. b. Korn Shell (KSH): A high-level programming language shell with advanced capabilities. c. Z Shell (Zsh): Offers unique features like login/logout watching, filename generation, and extended customization. d. Bourne Again Shell (Bash): The default shell for most Linux distributions, known for its wide adoption. e. Friendly Interactive Shell (Fish): Provides user-friendly features like web-based configuration and auto-suggestions.
    
6. What are the basic components of Linux?  
    The basic components of Linux include:  
    Kernel: The core component is responsible for managing hardware and software interactions. Shell: Acts as an interface for user communication with the kernel. GUI (Graphical User Interface): Provides a visual way for users to interact with the system through windows, icons, buttons, and text boxes. System Utilities: Software functions that allow users to manage the computer and perform various tasks. Application Programs: A collection of software designed for specific functions or tasks. What is BASH? BASH, or Bourne Again Shell, is a Unix shell and command processor created by Brian Fox for the GNU project. It serves as a replacement for the Bourne Shell and is interpreted rather than compiled. Users can issue commands and perform actions using BASH, making it a powerful tool for managing Linux systems.
    
7. What is the difference between Linux and Unix?  
    Key differences between Linux and Unix include:  
    Linux is available in both paid and free distributions, while Unix often involves various paid structures. Linux primarily uses a graphical user interface (GUI), while Unix is command-line oriented. Linux is portable and can run on different hardware platforms, whereas Unix is not as portable. Linux is developed by a global Linux community, while Unix is primarily developed by AT&T developers. Linux is generally free and available through the internet under GNU licenses, while most Unix-like operating systems are not free. Linux is commonly used on home-based PCs and phones, while Unix is commonly used in server systems.
    
8. What is LILO?  
    LILO, which stands for Linux Loader, is a boot loader used for Linux operating systems. It is responsible for loading the Linux operating system into the computer's main memory, allowing the system to start functioning.
    
9. What is CLI?  
    CLI, or Command Line Interface, is a text-based interface that allows users to interact with a computer by entering commands in the form of text lines. It interprets these text commands and converts them into actions executed by the operating system.
    
10. What is the advantage of Open Source?  
    The advantages of open-source software like Linux include:  
    Wide range of options: Users can modify and customize the software to suit their needs. Increased security: The open-source community continuously reviews and improves the software, making it more secure. Cost savings: Open-source software is often free to use, reducing the need for expensive licensing.
    
11. What is the disadvantage of Open Source?  
    Disadvantages of open-source operating systems can include:  
    Difficulty of use: Some open-source applications may lack user-friendly interfaces, making them challenging to set up and use. Compatibility issues: Open-source software may require specialized drivers for proprietary hardware, which can add to the cost and complexity. Liabilities and warranties: Open-source software may come with limited warranties and no liability protection, unlike proprietary software. Hidden costs: Some open-source software may appear free at first but could incur hidden costs during usage.
    
12. How do you open a command prompt when issuing a command?  
    You can open a command prompt by pressing CTRL+ALT+T or by searching for "terminal" in the menu search bar.
    
13. What is a swap space?  
    Swap space is used when the physical RAM memory is running low. It serves as virtual memory by moving inactive RAM pages to a dedicated swap partition or swap files, freeing up physical RAM for other tasks.
    
14. What is the GUI?  
    GUI, or Graphical User Interface, is a user interface that uses visual elements like windows, images, icons, and menus, which can be manipulated using a mouse. It provides a user-friendly way to interact with software and applications.
    
15. Explain File Permissions types in Linux.  
    In Linux, each file or directory has three types of permissions:
    
    Read: Allows users to read or view the contents of the file. Write Permits users to modify or edit the file. Execute Grants users the ability to execute or run the file as a program.
    
16. What are environmental variables?
    
    Environmental variables are dynamic values that affect the behavior of computer programs and processes. They provide information about the system's configuration and can be created, edited, saved, and deleted.
    
17. What are symbolic links?  
    Symbolic links are file system elements that redirect to another file using its path. The target file itself does not contain any data but instead points to another entry in the file system. If the target file is deleted, the symbolic link is also removed.
    
18. What are hard links?  
    Hard links are additional names for an existing file in Linux. Multiple hard links can be created for the same file, and they can even be used to create links to other hard links.
    
19. What is redirection?  
    Redirection in Linux refers to changing the standard input and output devices for commands or programs. This allows you to redirect the output of a command to a file or another program.
    
20. What are Daemons?  
    Daemons are background processes that accept service requests from other computers or processes. They run in the background and perform various tasks, such as network services or system maintenance.
    
21. Describe the root account.
    
    The root account is a privileged user account in Linux that has access to all files and commands. Root users have extensive system control and can perform tasks like installing software, changing file permissions, and system maintenance.
    
22. Explain the virtual desktop.  
    A virtual desktop provides an alternative method for managing multiple windows on a computer desktop. It allows users to organize and switch between different sets of open programs or applications, effectively creating multiple desktop environments within a single physical desktop.
    
23. What are the different modes when using the vi editor?  
    The vi editor has three main modes: Command Mode (Regular Mode): Used for navigation and manipulation of text. Insertion Mode (Edit Mode): Allows text to be entered or edited. Ex Mode (Replacement Mode): Used for advanced text manipulation and batch processing.
    
24. Explain File Permission groups in Linux.
    
    Linux assigns three permission groups to each file and directory: Owner: The owner has exclusive access to the file or directory and can control its permissions. Group: Group permissions apply to the group assigned to the file or directory and do not affect other users. All Users: Permissions in this group apply to all users on the system.
    
25. What is a File system in Linux?  
    A file system in Linux is a method for storing and managing data. It organizes data into files and directories and keeps track of their locations and attributes. Without a file system, an operating system wouldn't know how to manage files and data.
    
26. Explain different file system types in Linux.
    
    Linux supports various file system types, including Ext, Ext2, Ext3, Ext4, JFS, XFS, btrfs, ufs, autofs, devpts, ntfs, and swap. Each has unique features and is suitable for different use cases.
    
27. What are inode and process IDs?  
    Inode: An inode is a data structure in a file system that contains information about a file, such as its location, size, and permissions. Process ID: A process ID is a unique identifier assigned to each running process in an operating system. It allows the system to manage and track processes.
    
28. What are the Process states in Linux?  
    Linux processes can be in one of five states: New/Ready: A new process is created and ready to run. Running: The process is actively executing. Blocked/Wait: The process is waiting for input or a specific event. Terminated/Completed: The process has finished execution or was terminated by the operating system. Zombie: The process is deleted, but information about it remains in the process table.
    
29. Explain Process Management System Calls in Linux.
    
    Process management system calls in Linux include: fork(): Used to create a new process by duplicating the existing one. exec(): Executes a new program in the current process, replacing the existing program. wait(): Pauses a process until another specified process finishes. exit(): Terminates the current process. System calls to obtain process IDs include: getpid(): Retrieves the unique process ID. getppid(): Retrieves the unique parent process ID.
    
    **Linux Admin Interview Questions**
    
30. **Why LVM is required?**  
    LVM (Large Volume Management) is required to provide flexible storage management. Users can create, resize, and delete LVM partitions. It offers abstraction, flexibility, and control over storage resources. LVM allows for grouping existing storage devices and allocating logical units, making it an essential tool for efficient storage management.
    
31. **What is umask?**  
    Umask, short for "user file creation mode," controls the default file permissions when a user creates a file. It specifies restrictions on the newly created file, influencing file permission settings. The `umask` command can be used to view and set umask values, either symbolically or in octal representation.
    
32. **What are the different modes of Network bonding in Linux?**  
    Linux supports various network bonding modes to enhance network performance and reliability. These modes include balance-rr (Round-Robin), active-backup, balance-xor, broadcast, 802.3ad (dynamic aggregation), balance-tlb (transmit load balancing), and balance-alb (adaptive load balancing). Each mode offers unique features and is suitable for different network scenarios.
    
33. **How to check the default route and routing table?**  
    To check the default route and routing table in Linux, you can use various commands, such as `route -n`, `netstat -rn`, and `ip route show`. These commands display the routing information, including the default route, destination networks, and associated gateways.
    
34. **How to set the mask permanently for a user?**  
    To set the umask permanently for a user, you can use either octal representation or symbolic representation. You can modify the user's umask by editing configuration files, such as `.bashrc`, `.profile`, or `/etc/profile`, and adding the desired umask setting. This ensures that the umask value persists for that user.
    
35. **What is network bonding in Linux?**  
    Network bonding in Linux involves combining multiple network interfaces into a single virtual network interface. It aims to improve performance, redundancy, and load balancing. Bonding methods include balance-rr, active-backup, balance-xor, broadcast, 802.3ad, balance-tlb, and balance-alb, each offering different approaches to network aggregation.
    
36. **How to check which ports are listening in my Linux Server?**  
    To identify listening ports on a Linux server, you can use the `netstat --listen` or `netstat -l` commands. These commands provide a list of active network connections, including the open ports. You can use this information for network monitoring and troubleshooting.
    
37. **How to share a directory using NFS?**  
    To share a directory using NFS (Network File System), you need to edit the `/etc/exports` configuration file and add an entry for the directory you want to share. After modifying the configuration, you should restart the NFS service to make the directory accessible to other networked systems.
    
38. **What are the default ports used for SMTP, DNS, FTP, DHCP, SSH, and squid?** Default port numbers for common network services are essential to know. SMTP uses port 25, DNS uses port 53, FTP utilizes ports 20 and 21, DHCP operates on ports 67 and 68, SSH is on port 22, and Squid typically uses port 3128.
    
39. **How to lock a user account in Linux?**  
    Locking a user account in Linux enhances security. Various methods can be employed, such as disabling the password with the `passwd` command, expiring the user account using `usermod` or `chage`, or changing the user's shell to `/sbin/nologin`. These measures prevent unauthorized access to the account.
    
    These explanations cover the Linux Admin Interview Questions from 31 to 39.  
    here are explanations for the remaining Linux Admin Interview Questions:
    
40. **What is the 'ls' command and what does it do?**  
    The 'ls' command in Linux is a fundamental command used to list the files and directories in the file system. When used without any arguments, it displays the contents of the current working directory, listing files in alphabetical order. You can specify directory names as arguments to 'ls' to list the contents of specific directories. Additionally, you can list multiple directories by separating them with spaces.
    
41. **Where are the kernel modules located?**
    
    Kernel modules in Linux are typically located in the directory '/lib/modules/kernel-version/'. This directory stores information about the compiled kernel modules for the Linux system. You can also view the installed kernel modules using the 'lsmod' command.
    
42. **How to change the default run level in Linux?**  
    To change the default run level in Linux, you can use the 'init' command, followed by the desired run level number. For example, to set the default run level to 3, you can use the command 'init 3'. The run level determines the system's operational state and can affect services and processes that are started during system boot.
    
43. **What is the 'tail' command in Linux?**  
    The 'tail' command in Linux is used to display the last N number of lines from a given file or stream of data. By default, it prints the last 10 lines of the input, making it useful for monitoring log files or checking the most recent entries. You can specify the number of lines to display using the '-n' option, like 'tail -n 100 file.log' to show the last 100 lines.
    
44. **What is the 'env' command in Linux?**  
    The 'env' command in Linux is used to display a list of current environmental variables. It provides a snapshot of the current environment settings, including variables such as PATH, HOME, and more. Additionally, the 'env' command can be used to run another command in a modified environment by specifying variables and their values.
    
45. **What is the 'top' Command in Linux?**  
    The 'top' command in Linux is a dynamic system monitoring utility. It displays real-time information about running processes, system performance, and resource usage. It helps users monitor CPU usage, memory usage, and other system metrics. You can use 'top' to identify processes that consume system resources and make informed decisions on resource management.
    
46. **What is the 'netstat' command in Linux?**  
    The 'netstat' command in Linux provides various information about network connections, routing tables, network interfaces, and more. It is a powerful tool for network monitoring and diagnostics, allowing users to view open ports, active network connections, and routing information.
    
47. **What is the 'lsof' command in Linux?**  
    The 'lsof' command stands for "List of Open Files" and is used to identify which files are currently open by processes on the system. It can provide detailed information about file descriptors, network connections, and other resources held by processes. 'lsof' is valuable for troubleshooting issues related to open files and processes.
    
48. **Explain the 'chmod' command.**  
    The 'chmod' command in Linux is used to change the permissions of files and directories. It allows users to modify file permissions to control who can read, write, and execute files. 'chmod' uses numerical representations (e.g., 755) or symbolic notations (e.g., u+rwx) to set permissions. This command is crucial for managing access control and security on Linux systems.
    
49. **What is the 'grep' command in Linux?**  
    The 'grep' command is a text-searching utility used to search for patterns or regular expressions in text files or streams of data. It helps users find specific lines or data that match the given pattern. 'grep' is a powerful tool for filtering and extracting information from files and is commonly used for tasks like log analysis and text processing.
    
50. **What is the 'ps' command in Linux?**  
    The 'ps' command in Linux is used to display information about currently running processes on the system. It provides details about process IDs, terminal sessions, and various process attributes. 'ps' helps users monitor and manage processes, making it a valuable tool for system administrators.
    
51. **Explain the 'chown' command.**  
    The 'chown' command, short for "change owner," is used to modify the ownership of files and directories in Linux. Users can change the owner and group of a file using 'chown,' typically requiring superuser (root) privileges. It is a crucial command for managing file permissions and access control.
    
52. **How to remove a file or directory from the system in Linux?**  
    To remove a file or directory from the system in Linux, you can use the 'rm' command. For files, you can simply use 'rm filename' to delete a specific file. For directories, you can use 'rm -r directoryname' to recursively remove a directory and its contents. Be cautious when using the 'rm' command, as it permanently deletes files and directories.
    
53. **What is the 'mkdir' command in Linux?**  
    The 'mkdir' command in Linux is used to create directories (folders) in the file system. It allows users to create one or multiple directories at once. You can specify directory names as arguments and use options to set permissions and other attributes while creating directories. 'mkdir' is essential for organizing and structuring the file system.
    
54. **How to exit from vi editors?**  
    To exit from a vi editor, you can use various commands:
    
    * To save changes and exit, you can use ':wq' or ':x'.
        
    * To exit without saving changes, you can use ':q!'.
        
    * To save changes without exiting, you can use ':w'.
        
    * To navigate and edit the file, you can use 'i' to enter insert mode and 'Esc' to return to command mode.
        
        1. **Explain the 'rmdir' command in Linux.**  
            The 'rmdir' command in Linux is used to remove directories that are empty. It is specifically designed to delete directories without any files or subdirectories inside. If a directory has contents, 'rmdir' will not work, and you'll need to use 'rm -r' to remove it along with its contents.
            
    
    **56\. Enlist some Linux file content commands.**  
    Commands for viewing file content in Linux include:
    
    * 'cat': Concatenates and displays file contents.
        
    * 'head': Displays the top lines of a file.
        
    * 'tail': Shows the last lines of a file.
        
    * 'more': Displays content in a pager form for easy reading. These commands are essential for viewing and manipulating file content.
        
    
    **57\. How to delete information from a file in vi?**  
    To delete information from a file in a vi editor, you can use various commands in command mode:
    
    * 'x' deletes the current character.
        
    * 'dd' deletes the current line.
        
    * 'd' followed by a movement command (e.g., 'dw' to delete a word) can delete specific portions of text.
        
    
    **58\. What is meant by internal commands and external commands?**  
    Internal commands are those that are built into the shell or command interpreter and are executed directly by the shell itself. Examples include 'cd' for changing directories and 'echo' for displaying messages.
    
    External commands are standalone executable programs or scripts that are not part of the shell. These commands are separate files, and when you run them, they create a new process. Examples include 'ls' for listing files and 'grep' for searching text in files.
    
    1. **Why do we use LINUX?**  
        Linux is used for several reasons, including:
        
    
    * High Stability: Linux is known for its stability, reliability, and resistance to crashes.
        
    * Security: It provides robust security features, protecting against viruses and malware.
        
    * Ease of Use: Linux is user-friendly, with software repositories for easy installation and updates.
        
    * Hardware Compatibility: Linux can run on various hardware platforms efficiently.
        
    * Open Source: It is open-source, allowing users to access and modify the source code, fostering community development.
        
    
    **60\. What are the features of the Linux operating system?**  
    Features of the Linux operating system include:
    
    * Portability: Linux can run on various hardware architectures.
        
    * Open Source: It's an open-source operating system with accessible source code.
        
    * Multi-User: Multiple users can use the system simultaneously.
        
    * Multiprogramming: Multiple programs can run concurrently.
        
    * Shell: Linux provides a command-line interface for executing commands.
        
    * Security: It offers authentication, authorization, and data encryption for security.
        
    
    **61\. Differentiate between BASH and DOS?**  
    Differences between BASH (Bourne-Again Shell) and DOS (Disk Operating System) include:
    
    * BASH is case-sensitive, while DOS commands are not.
        
    * BASH uses a forward slash '/' as a directory separator, while DOS uses a backward slash ''.
        
    * BASH has different naming conventions for files, whereas DOS follows case-insensitive naming.
        
    * BASH uses the escape character '', while DOS uses the forward slash '/' as an escape character.
        
    
    **62\. What is meant by internal commands and external commands?**  
    Internal commands are built into the shell and executed directly by the shell. External commands are standalone executable programs or scripts that create new processes when run.
    
    **63\. Enlist some Linux distributors (Distros) along with their usage.**  
    Popular Linux distributions (Distros) and their common usage include Linux Mint (for stability), Debian (known for robustness and stability), Ubuntu (both desktop and server editions), openSUSE (user-friendly), and Manjaro (offering a pleasant experience for users).
    
    These explanations cover the Linux Admin Interview Questions from 53 to 63.
    
    1. **What is meant by PIPE in Linux?**  
        In Linux, a "PIPE" is a mechanism used to connect the output of one command to the input of another. It allows you to create a data flow from one command to another, enabling you to process and manipulate data sequentially. The vertical bar symbol (|) is used to represent the pipe operator. For example, you can use `command1 | command2` to take the output of `command1` and pass it as the input to `command2`.
        
    2. **Explain the features of a Stateless Linux Server.**  
        A Stateless Linux Server is a server that doesn't maintain any local state information on the machine itself. Instead, it relies on external sources for state information, such as network configuration and system snapshots. Features of a Stateless Linux Server include storing the system prototype, snapshots, and home directories, and using LDAP for managing system states.
        
    3. **What is a Zombie Process?**  
        A Zombie Process is a state in the process lifecycle where a process has terminated, but its entry in the process table hasn't been removed. This typically occurs when the parent process hasn't yet collected the exit status of its terminated child process using the `wait` system call. Zombie processes occupy system resources but don't perform any useful work. They are eventually removed from the process table once the parent process collects the exit status.
        
    4. **Explain the work of the Ctrl+Alt+Del key combination on the Linux operating system.** In Linux, the Ctrl+Alt+Del key combination is used to initiate a system reboot. When pressed, it triggers a graceful system restart without displaying a confirmation message. This combination is a keyboard shortcut to initiate the reboot process.
        
    5. **Describe how a parent and child process communicate with each other.** Parent and child processes in Linux can communicate with each other using various inter-process communication (IPC) mechanisms, such as pipes, signals, sockets, shared memory, and message queues. These mechanisms allow processes to exchange data and coordinate their activities. For example, a parent process can send signals to its child to instruct it to perform specific actions.
        
    6. **What is a Stateless Linux Server?**  
        A Stateless Linux Server is a server configuration in which the server doesn't maintain local state information. Instead, it relies on external sources for system configuration and state data. This approach simplifies server management, as all state information is managed externally, making servers easier to manage and scale.
        
    7. **Why is Linux considered more secure than other operating systems?**  
        Linux is considered more secure than some other operating systems for several reasons, including its permission system, limited user accounts, strong community support, use of iptables for firewall and security, diverse working environments, and comprehensive logging. Additionally, the open-source nature of Linux allows users to review and enhance security, making it less vulnerable to threats.
        
    
    These explanations cover the Linux Admin Interview Questions from 64 to 70. If
    
    1. **What is the** `cat` **command in Linux?**  
        The `cat` command in Linux is used to concatenate and display the contents of files. It is a versatile utility that allows you to view the contents of one or multiple files, create new files, or combine the contents of files. It's commonly used for displaying the contents of text files in the terminal.
        
    2. **What is the** `tail` **command in Linux?**  
        The `tail` command in Linux is used to display the last part of a file, typically used to show the tail end of log files. By default, it displays the last 10 lines of a file, but you can specify the number of lines to show using the `-n` option. It is useful for monitoring log files in real-time.
        
    3. **What is the** `grep` **command in Linux?**  
        The `grep` command in Linux is used for searching text patterns in files. It stands for "global regular expression print." You can specify a pattern and `grep` will search for that pattern in the given files and display lines that match the pattern. It's a powerful tool for text searching and filtering.
        
    4. **What is the** `df -i` **command used for?**  
        The `df -i` command is used to display the number of free inodes on mounted file systems. Inodes are data structures used by the file system to represent files and directories. This command helps you monitor the availability of inodes on your file systems, which is essential for managing large numbers of files.
        
    5. **How do you kill the program using one port in Linux?**  
        To kill a program using a specific port in Linux, you can use the `fuser` command with the `-k` option.  
        This command will identify the process using port 8000 and terminate it.
        
    6. **How do you limit memory usage for commands?**  
        You can limit memory usage for commands using the `ulimit` command. For example, to limit the memory usage to 1 MB, you can use:
        
    7. **What does** `(cd dir && command)` **do?**  
        The `(cd dir && command)` command changes the current directory to `dir` and then executes the specified `command`. This is useful for running a command within a specific directory context without permanently changing the working directory.
        
    8. **What does the** `push` **command do?**  
        The `push` the command isn't a standard Linux command. It may refer to a custom script or function in a specific environment, but it's not part of the core Linux command set.
        
    9. **How do you get the full path of a file in Linux?**  
        You can get the full path of a file in Linux using the `readlink` command with the `-f` option. For example:
        
    
    This command will display the full path of the file `file.txt`.
    
    1. **What is the** `du -s * | sort -k1,1rn | head` **command used for?**  
        The `du -s * | sort -k1,1rn | head` command is used to list directories and their disk usage (in kilobytes) in the current directory and sort them in reverse order by size. The `head` command then displays the top directories with the largest disk usage.
        
    2. **How do you check resource usage?**  
        To check resource usage for a specific command, you can use the `/usr/bin/time` command followed by the command you want to monitor.
        
    
    This command will provide detailed resource usage information for the `ls` command.
    
    **81\. How do you run a command every time a file is modified?** You can use the `inotifywait` command in a loop to monitor changes to a file and run a specific command when the file is modified.
    
    This will continuously watch for changes `document.tex` and run the `make` command whenever it's modified.
    
    These explanations cover the Linux Admin Interview Questions from 71 to 82.