---
title: "3. Docker Container Orchestration"
datePublished: Fri Oct 13 2023 14:56:30 GMT+0000 (Coordinated Universal Time)
cuid: clnoqeu2c000709l7gq04ffq2
slug: 3-docker-container-orchestration
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697208900033/1c9f3cee-fa44-4f01-af88-5e88d7a399bd.png
tags: docker, devops, devops-articles, container-orchestration, devopscommunity

---

#### Container Orchestration:

* When we are running our application in our container technology, we need to have some control over it, so that we can see zero downtime deployments, also how can scale individual applications, we need something to control that.
    
* Kubernetes is made open source to control multiple containers running on multiple machines we need some orchestrator, and that orchestrator is Kubernetes.
    
* Docker and Kubernetes are interrelated, Kubernetes runs containers and the best container technology is Docker.
    
* The most popular container technology is Docker
    
* Container Orchestration (Kubernetes)
    
* Long back If you want to run an Apache server/Jenkins, take a Linux machine, in it you need to install software, Jenkins requires Java so you need to install Java, in that you can run Jenkins.
    

#### Running multiple web servers on the same machine:

It is possible but difficult to run two Jenkins, on the same Machine.

Let's see how Docker does this,

Go to play with Docker

![](https://t9002062579.p.clickup-attachments.com/t9002062579/66440332-2a54-4287-bc46-e015f5f1fe2f/docer1.png align="left")

Click on login to the site

![](https://t9002062579.p.clickup-attachments.com/t9002062579/99fb445e-e0f2-42f6-91f8-c7a466bc258d/docker2.png align="left")

sign in/log in with your credentials

![](https://t9002062579.p.clickup-attachments.com/t9002062579/3eb6532f-ee41-4fa6-85ed-eb3ffe5201ac/docker3.png align="left")

click on Start and get started.

![](https://t9002062579.p.clickup-attachments.com/t9002062579/af7e9d0f-086f-46de-8310-93cbae77a9f7/docker4.png align="left")

The interface looks like this and gets started working.

Go to add new instance, it will expire in 3:30 hours time duration.

![](https://t9002062579.p.clickup-attachments.com/t9002062579/eb38b304-f322-4a6f-805c-973aa859bf13/docker5.png align="left")

Then enter the commands:

the help command will help give you the list of commands needed to run

![](https://t9002062579.p.clickup-attachments.com/t9002062579/5b030f52-c268-4103-a532-bdfe459b5b28/image.png align="left")

need to run the Jenkins server, this command will help to get into it

![](https://t9002062579.p.clickup-attachments.com/t9002062579/5820e2ad-31de-48ba-98f3-5028c2480974/image.png align="left")

if you want to run the nginx server then enter the command.

if you want to run nginx servers on the same machine then use the commands

![](https://t9002062579.p.clickup-attachments.com/t9002062579/401ff888-46c3-4d27-aa6f-e3df8a8255aa/image.png align="left")

To know how much memory the nginx takes go to this command

![](https://t9002062579.p.clickup-attachments.com/t9002062579/367f5689-cd70-4623-9c61-7ed048585cd0/image.png align="left")

You can run two nginx servers on the same machine

![](https://t9002062579.p.clickup-attachments.com/t9002062579/410bc5f7-ebc7-453c-afaa-0c4cdfbcc44c/image.png align="left")

without installing Java we can run servers as shown,

![](https://t9002062579.p.clickup-attachments.com/t9002062579/58a6e38b-e241-4e4f-9f0b-29d97d1330a4/image.png align="left")

It is possible to run multiple servers without installing Java because of the container technology.