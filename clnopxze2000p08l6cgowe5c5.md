---
title: "2. Architecture of an Application & Micro-Services"
datePublished: Fri Oct 13 2023 14:43:23 GMT+0000 (Coordinated Universal Time)
cuid: clnopxze2000p08l6cgowe5c5
slug: 2-architecture-of-an-application-micro-services
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697208029591/fffefbf9-0169-4cce-a266-dfa3b39bdeb4.png
tags: microservices, architecture, devops, devops-articles, microservice-architecture

---

### **Servers are of three types:**

Web Servers, Application Servers, Database Servers

* Datacentres have a collection of servers each server organized in racks.
    
* Each rack gets a power supply and network connection, and each rack has TORS (Top of the rack switch) to distribute  the network to multiple servers in a rack
    
* In racks, we use blade servers.
    

### **Data Centres:**

* on-premise, cloud.
    
* Applications work on data servers these are all about infrastructure
    
* Applications can be deployed(working) on the production servers
    
* Capex (capital expenditure), Opex (operational expenditure), and ROI (Return on investment) will take a lot of time.
    
* Directly installing OS on physical servers is not encouraged so we use Hypervisors(like VMWare)
    
* Hypervisor is a  software that is used to create Virtual Machines
    
* There are two generations of Hypervisors.
    
* Virtual machines are created on physical servers with some hosts and guests
    
* Hypervisors help to create virtual machines
    
* BCDR (Business Continuity and Disaster management)
    

#### The Architecture of an Application:

* The database is not meant for storing Images, files, or videos they can be stored in the image store.
    
* The standby database is used to support the database if it is not working.
    
* whenever you want to access the website, the request goes to the app server, all the business projects are in the business layer, and send the request to the database layer.
    
* when the server shutdown the users can't access the site, and at downtime, the application can't access it.
    
* Do the deployment first, if it is working then apply it to the server then the application is working well.
    
* some applications want to run in any cloud/on-premises. The applications will run on any server, whatever the cloud it may be.
    
* Any organization wants min. requirements like portability, deployment of new features, accessibility, zero downtime deployments, and cross-platform, typically having fewer downtimes and faster deployments.
    

### Micro-Services

* The API layer acts as an adapter between the business layer & the mobile app, HTML, CSS Java script
    
* Running all the applications in one server is called Monoliths.
    
* According to the organization, Decomposing applications into small multiple business services and running them individually is called microservices.
    
* It's easy to work on individual services, rather than working on the whole application, it's only possible when the whole application breakdown into multiple servers ie microservices.
    
* Break down your applications into smaller components, so that it is easily maintainable, if you want to make changes you can easily make a change to a particular service, it will not affect the whole application & it will not take much time to restart the particular service.
    
* If you want to reuse one part of an application, no need to rewrite the code, take the service you need & use it one benefit of it is how Amazon has built identity services like Amazon Prime, Amazon Music and Netflix, and Google Works which run in common. Google does the identity services.
    
* If I want to reuse any part of my application, there is no need to rewrite the code, just take the service & use it over there.
    

#### Advantages of Microservices:

* microservices are useful in Application deployments easy
    
* Restarting the smaller service is much faster than restarting the whole application.
    
* Updation also takes less time for any particular microservices.
    
* Re-using microservices is much easier.
    
* microservices can use individual programming languages rather than the whole application because whatever technology better fits the problem to solve can be used. because all of the microservices can speak over communication protocols that are the same for every language.
    
* They can work on any which is TCP/HTTP/grpc (which can work on any language). which can work on any rapid application development.
    
* working on smaller parts of the application & build with end-to-end layers.
    
* web applications run on web servers, this web server will run on some servers which have some CPU, memory, RAM
    
* Whenever you request to web server from the web it creates a thread, every thread has some CPU and RAM
    
* when multiple users log in to multiple servers, multiple threads will be created.
    
* when the servers are less & the traffic is more & communicating with HTTP protocol, it will not stay longer, whatever the application we configured if the server does not respond it will give an error message the request has been timed out.
    
* Trying to run the whole of your application on one web server, needs much CPU/RAM but using microservices takes less space.
    
* Running a huge application on a single server needs scaling the whole application, which takes much RAM/CPUs, rather than this individual service no need to scale with huge servers, as it takes less CPU/RAM
    
* Scaling is possible, by parts of an application not by increasing the whole application, where there is a demand.
    
* scaling for microservices is much cheaper & easier compared to scaling monolith.