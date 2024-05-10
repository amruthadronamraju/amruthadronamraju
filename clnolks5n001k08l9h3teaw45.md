---
title: "DevOps Basics"
datePublished: Fri Oct 13 2023 12:41:09 GMT+0000 (Coordinated Universal Time)
cuid: clnolks5n001k08l9h3teaw45
slug: devops-basics
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697200808048/9f4fc8da-097a-4e1c-89ef-17f01f0e423e.png
tags: cloud-computing, devops, devops-articles, devopsbasics, devopscommunity

---

DevOps essentials

Linux

Aws  
Continuous Deployment:  
. The step-by-step pipeline process when the developer develops the code in VCS for the production environment is called continuous deployment.  
  
When the developer develops the code it sent to the VCS by using git, it cannot be sent to the production directly

Whatever code has been written and converted into some understandable language / installed some application/server which can understand the build/package that is sent to performance testing, then sent to the UAT/Pre-Production, before giving it to the customer the developer has to check the product has no faults in the production environment.  
  
First, the package is sent to the system test environment & when executed all the system tests & are passed to performance testing once it is successful it is sent to UAT/ pre-production to do all the tests once everything is done without faults/bugs it was sent to the production to deliver the product to the customers.

According to the company's need, the production may have a few more steps to test the product/application for more quality.

when you try to automate the moment developers develop the code till it reaches production, this pipeline process is called continuous deployment.

The process to reach from VCS to the production environment is called continuous deployment.  
  
create a pipeline that tries to automate all the environments but not production, this is called continuous Delivery.

Deployment takes you to production, Delivery will not take you to production.

when the developers develop the code & send it to VCS & then build the package & make a small test whether it is working or not & send feedback to the developer on whether the code is working/not this is called continuous integration.

Continuous Deployment (Automate Everything)

Continuous Delivery (Automate everything apart from production)

Continuous Integration (Not automating everything, doing some basic checks & giving feedback to the developer.

for VCS the developers submit the code to git.

maven which helps in developing Java applications  
  
The command that you want to Update PowerShell:

* **Servers are of three types:** Web Servers, Application Servers, Database Servers
    
* Datacentres have a collection of servers each server organized in racks.
    
* each rack gets a power supply and network connection, and each rack has TORS (Top of the rack switch) to distribute  the network to multiple servers in a rack
    
* In racks, we use blade servers.
    
* Command to kill all the notepads at a time:
    
    ![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhZ5DSsYdqRyL7fxQB9MBeMyyiQ84SnxIh69a9jFV33ARA6oZ6uBQPqfs8p1cpOnQG0wB1JBi3S6cl-QjfO2046ek-GG0z2TTo_66UepKmIZ6vKKmm4z9Dp6ugNyd7td-6G_ZQk67glDTlc8XmYoxGWiTtxtWJx2fTgPKL_n-5PSd3m3a4vm3RnY1mo/w640-h326/2.png align="left")
    
* Data centres: on-premise, cloud                 ·
    
* Applications work on data servers these are all about infrastructure
    
* Applications can be deployed(working) on the production servers
    
* Capex (capital expenditure), Opex (operational expenditure), and ROI (Return on investment) will take a lot of time.
    
* Directly installing OS on physical servers is not encouraged so we use Hypervisors (like VMWare)
    
* Hypervisor is a  software that is used to create Virtual Machines
    
* There are two generations of Hypervisors.
    
* Virtual machines are created on physical servers with some hosts and guests
    
* Hypervisors help to create virtual machines
    
* BCDR (Business Continuity and Disaster management)
    
    ![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhg7oIUdytxLWhnO6MTHG4-rsvwm63036_TKUQCvWitQGrQtK32Y59w3hSwLx_9aekHOSJsFcyBSvPTypeRqs8Rt4CiFyX4po6Soz5rmLVkNkVajVF0BapOtpgerAmuU9tGMLsczBqiavd_bLKXaAYPvB55NR5Ln-OmCr_3cGgwgtl9qDkk_cZPlxeD/w640-h370/update.powershellcommand.png align="left")
    
    command to update Windows Powershell by copying the path of the exe file and pasting it into the terminal and running.