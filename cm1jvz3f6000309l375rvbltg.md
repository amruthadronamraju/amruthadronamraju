---
title: "Linux Key Notes-1"
datePublished: Thu Sep 26 2024 22:49:15 GMT+0000 (Coordinated Universal Time)
cuid: cm1jvz3f6000309l375rvbltg
slug: linux-key-notes-1
tags: linux-for-beginners

---

key Linux system management concepts, particularly file ownership, permissions, and process management. Here's a summary of the core ideas, broken down for clarity:

### **File Ownership and Permissions**

1. **File Creation and Ownership**:
    
    * When a file is created in any operating system, including Linux and Windows, the user who creates the file automatically becomes its owner.
        
    * In Linux, the file owner can be identified using commands like `ls -l` to view the file ownership and permissions.
        
2. **Permissions in Linux**:
    
    * **Three levels of users**:
        
        * **Owner (User)**: The person who created the file and typically has full control.
            
        * **Group**: Other users in the same group as the owner.
            
        * **Others**: All other users on the system who are not the owner or in the owner's group.
            
    * **Permissions**: There are three types of permissions:
        
        * **Read (r)**: Allows reading the file.
            
        * **Write (w)**: Allows modifying or deleting the file.
            
        * **Execute (x)**: Allows executing the file (if it's a script or program).
            
    * The permissions are shown as a set of three characters for each level (user, group, others). For example, `rwxr-xr--` would mean:
        
        * The owner has read, write, and execute permissions.
            
        * The group has read and execute permissions.
            
        * Others have only read permissions.
            
3. **Changing Ownership and Permissions**:
    
    * Use the `chown` command to change file ownership:
        
        * `sudo chown user:group filename`
            
    * To change file permissions, use the `chmod` command with numerical representation (e.g., `chmod 755 filename`):
        
        * **7** = read (4) + write (2) + execute (1) = full access.
            
        * **5** = read (4) + execute (1) = read and execute only.
            
    * Special users like `root` have full control, but a regular user might need to use `sudo` to perform administrative tasks.
        

### **Process Management in Linux**

1. **Processes and Process IDs (PID)**:
    
    * Every task running in Linux (whether it's a user command or a system process) is assigned a unique **process ID (PID)**.
        
    * Linux uses these IDs to keep track of all activities in the system.
        
    * You can view running processes using the `ps` or `top` commands, which will show each process's ID, along with details like CPU and memory usage.
        
2. **Types of Processes**:
    
    * **Foreground processes**: These are interactive processes initiated by the user (e.g., opening a terminal or running a command like `ls`).
        
    * **Background processes**: These are non-interactive and run in the background, often system services (daemons) or tasks started by users (e.g., `cron` jobs).
        
3. **Terminating Processes**:
    
    * Processes can terminate naturally when their task is complete (e.g., after running a command).
        
    * If a process becomes unresponsive, you can manually kill it using the `kill` command along with its PID:
        
        * `kill PID` sends a termination signal to the process.
            
        * `kill -9 PID` forces termination if the process doesn’t respond to the default signal.
            
    * You can find the PID of a running process with `ps aux | grep processname` or use `top` or `htop` to monitor real-time system activities.
        
4. **Handling Hung Processes**:
    
    * In cases where a system or application hangs (similar to Task Manager in Windows), Linux allows you to use commands like `kill` or `xkill` to forcefully terminate the application or process causing the issue.
        

### **Scenario in Multi-Project Environment**:

* In an organization, multiple projects may run on the same Linux server. Permissions management is critical to ensure that:
    
    * Project 1's team can't interfere with Project 2's files or processes.
        
    * Proper file permissions and user groups ensure that teams can work securely without overlapping responsibilities or privileges.
        
* By understanding these concepts of ownership, permissions, and process control, users can effectively manage tasks and files within Linux systems. Do you have any specific questions on how to apply these concepts in real-world scenarios?
    

### 1\. **Port Numbers and IP Addresses:**

* Port numbers are like apartment numbers in a building, and the IP address is like the building’s address. Together, they help you reach a specific service or database on a server.
    
* Each service (like Tomcat, Nginx, MySQL) has a unique default port number, but you can change it if needed.
    
* You can install multiple databases or tools on the same server, but they must have different port numbers.
    
* **Example:** Tomcat might use port 8080 by default, but if it's already taken, you can change it to 8081 or something else.
    

### 2\. **Managing Port Numbers:**

* You cannot use the same port number for two services on the same server. If you try, it will cause a conflict, and the system won’t allow it.
    
* Always check which ports are in use before assigning a new port to a service. You can use commands like `netstat` to see which port numbers are already being used.
    

### 3\. **Processes and Port Mapping:**

* Every running tool or service has a **process ID** and a **port number**. These two are connected.
    
* The operating system assigns a process ID to each running task, but you, as the user, decide which port number to assign to a tool.
    
* If a process stops or is killed, the port it was using becomes free.
    

### 4\. **Monitoring Servers:**

* On a Linux server, you can monitor performance using the `top` command. This is similar to the Task Manager on Windows.
    
* The **CPU usage**, **memory usage**, and **load average** tell you how busy or overloaded your server is.
    
* **Load Average** shows you how many tasks are waiting to be processed by the CPU. If the load is low (close to 0), the system is performing well.
    
* High **CPU usage** or **memory usage** means the server is working hard, and you should monitor for slowdowns.
    

### 5\. **Process Utilization:**

* You can check which processes are using the most CPU or memory. The processes using the most resources are shown at the top when you run the `top` command.
    
* If a process is using too much CPU or memory, you can find its process ID and decide whether to stop or kill it.
    

### 6\. **Changing Port Numbers:**

* Even though most tools come with default port numbers, you can always change the port to avoid conflicts.
    
* When setting up projects, port numbers and IP addresses are usually decided during the design phase. But it’s always a good idea to double-check and verify which ports are being used.
    

### 7\. **System Performance and Uptime:**

* The system's **uptime** tells you how long it has been running without a restart.
    
* It’s important to monitor your server’s health, especially if it is running a lot of processes, as this can lead to slowdowns or crashes.
    

### 8\. **How to Find Port-Process Mapping:**

* Use commands like `netstat -nlp` to find out which process is using a particular port. This helps you identify who or what is using that port so you can take action.
    

### 9\. **Basic Commands:**

* `ps -ef`: Shows all running processes.
    
* `netstat`: Shows network connections and port usage.
    
* `top`: Shows system performance (CPU, memory, and processes).
    

### 10\. **Practical Tips:**

* Always check the load on your server. Low load means the system is running smoothly.
    
* Avoid running too many processes at the same time to prevent system crashes or slowdowns.
    
* When working in a team, ensure everyone uses the correct port numbers and follows the design documents.
    

By focusing on these points, you will have a solid understanding of how port numbers, processes, and system monitoring work, especially in Linux environments.