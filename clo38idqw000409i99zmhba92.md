---
title: "AWS Load Balancer Interview Q/A"
datePublished: Mon Oct 23 2023 18:31:55 GMT+0000 (Coordinated Universal Time)
cuid: clo38idqw000409i99zmhba92
slug: aws-load-balancer-interview-qa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1699031378085/e368bcb5-cbeb-4033-ba93-96e62ea2b0db.png
tags: aws, load-balancer, aws-interview-question-and-answers, aws-elastic-load-balancer, amazonloadbalancer

---

1. **What is an Elastic Load Balancer (ELB)?**  
    An Elastic Load Balancer (ELB) is a service in Amazon Web Services (AWS) that automatically distributes incoming application traffic across multiple instances to ensure high availability and scalability. It plays a crucial role in load balancing, which optimizes resource utilization and ensures that applications can handle traffic efficiently.
    
2. **What are the key features provided by Elastic Load Balancer (ELB)?**
    
    * *High availability*: ELB ensures that traffic is directed to healthy instances, increasing application reliability.
        
    * *Automatic scaling*: ELB can work in conjunction with AWS Auto Scaling to adjust the number of instances based on traffic load.
        
    * *Security*: It can be used within Amazon Virtual Private Cloud (VPC) for stronger network security.
        
3. **How does AWS Elastic Load Balancing work?**  
    ELB accepts incoming traffic, and route requests to registered targets (e.g., EC2 instances), and monitors the health of these targets. It ensures that traffic is only sent to healthy targets and can detect and handle unhealthy instances.
    
4. **What is a target group in AWS Load Balancing?**  
    A target group is used to specify where traffic should be directed by a load balancer. It can include EC2 instances, fixed IP addresses, or AWS Lambda functions. When setting up a load balancer, you configure listener rules to direct traffic to one or more target groups.
    
5. **What is the difference between auto-scaling and ELB?**  
    Auto-scaling dynamically adjusts the number of instances based on traffic load, while ELB balances traffic across multiple instances to ensure even distribution. Auto-scaling and ELB are related because scaling policies often consider the load balancer's serving capacity as one of the metrics.
    
6. **How do you configure session affinity in an AWS Elastic Load Balancer?** Session affinity, or sticky sessions, ensures that a user's requests are consistently handled by the same server during their session. To configure this in an AWS Elastic Load Balancer, you create the load balancer, enable session affinity, specify the session duration, and configure your web servers to use the load balancer as their session affinity provider.
    
7. **Explain NLB in AWS.**  
    AWS Network Load Balancer (NLB) is a service that distributes end-user traffic across multiple cloud resources for low latency and high throughput. It can route traffic to healthy targets and offers similar load-balancing capabilities to other load balancers in AWS.
    
8. **What are the different types of load balancers?**  
    The three main types of load balancers are hardware, software, and cloud load balancers. Hardware load balancers are physical devices, software load balancers run on servers, and cloud load balancers are hosted in the cloud and are suitable for cloud-based applications.
    
9. **What are the types of load balancers in Elastic Load Balancing?**  
    Elastic Load Balancing provides four types of load balancers: Application Load Balancers, Network Load Balancers, Gateway Load Balancers, and Classic Load Balancers. Each serves specific use cases and offers different capabilities.
    
10. **How can you assign a static IP address to an ELB?**  
    To assign a static IP address to a Network Load Balancer, you can allocate Elastic IP addresses in the Amazon Elastic Compute Cloud (Amazon EC2) console. Then, when creating the Network Load Balancer, you can select an Elastic IP address to be assigned to its interfaces.
    
11. **What is a VPC load balancer?**  
    A VPC load balancer is an Elastic Load Balancer (ELB) provisioned within a Virtual Private Cloud (VPC). It can have security groups assigned to it, be placed in VPC subnets, and be used without the need for public IP addresses on the registered instances.
    
12. **Which ELB component is responsible for monitoring the Load Balancers?**  
    The Controller Service is responsible for monitoring the Load Balancers.
    
13. **What are the different types of load balancing options provided by Amazon Elastic Load Balancing (ELB)?**  
    Amazon Elastic Load Balancing provides three main types of load balancers: Application load balancing, Network load balancing, and Classic load balancing. Each type is suitable for different use cases and has distinct features.
    
14. **Can we have an internal or private ELB as the origin in CloudFront?**  
    No, CloudFront does not support using an internal or private Elastic Load Balancer (ELB) as an origin. It requires a publicly accessible origin for content delivery.
    
15. **What are the different types of AWS Load Balancers?**  
    AWS Load Balancers come in three types: Application Load Balancers, Network Load Balancers, and Classic Load Balancers. Each type is optimized for specific use cases and offers varying features.
    
16. **Are you using Auto Scaling for your EC2 instances? How have you configured the Auto scaling policy?**  
    Yes, Auto Scaling is used to dynamically adjust the number of EC2 instances based on load. The configuration of the Auto Scaling policy includes setting maximum and minimum numbers of instances based on specific criteria.
    
17. **What is the best way to set up a load balancer in a cloud environment like Amazon Web Services?**  
    The best way to set up a load balancer in a cloud environment like AWS is to combine Elastic Load Balancers (ELBs) with Auto Scaling groups. ELBs distribute traffic evenly, while Auto Scaling ensures there are enough instances to handle the traffic load.
    
18. **List the types of techniques used by load balancers.**  
    Load balancers use various techniques, including Round Robin, Weighted Round Robin, Least Connection, Weighted Least Connection, Resource-Based (Adaptive), Resource-Based (SDN Adaptive), Fixed Weighting, and Weighted Response Time, to optimize traffic distribution.
    
19. **What is the difference between clustering and load balancing?**  
    Clustering groups servers into a single system for redundancy, while load balancing distributes workloads across multiple computing resources. Clustering deals with server availability, while load balancing optimizes resource utilization.
    
20. **What's the difference between Active and Passive Health Checks?**  
    Active health checks are initiated by the load balancer, while passive health checks are initiated by the server. Active health checks are more accurate as the load balancer directly tests server responsiveness, while passive checks rely on server behavior.
    
21. **Why is fault tolerance important when using a load balancer?**  
    Fault tolerance is essential when using a load balancer to ensure high availability. It provides redundancy and ensures that the load balancer itself does not become a single point of failure. Redundant load balancers can step in if one fails.
    
22. **When would you choose a Layer 4 vs a Layer 7 load balancer?**  
    You would choose a Layer 4 load balancer when routing based on IP and port information is sufficient. Layer 7 load balancers are selected when more advanced routing based on content, such as HTTP headers, is needed.
    
23. **Can you give examples of real-world use cases for DNS load balancing?**  
    DNS load balancing is used to distribute traffic across multiple servers to:
    
    * Balance the load on a high-traffic website.
        
    * Provide redundancy in case of server failures.
        
    * Route traffic to the closest server geographically for reduced latency.
        
24. **Can you explain how DNS load balancing works and how it differs from other load balancing methods?**  
    DNS load balancing distributes traffic using DNS records, directing users to different server IP addresses. It differs from other load-balancing methods as it relies on DNS rather than a dedicated load balancer to make routing decisions.
    
25. **What are some advantages of using a reverse proxy as opposed to a forward proxy with load balancing?**  
    Advantages of using a reverse proxy include simplified firewall configuration, improved security, caching, compression, and the ability to handle client requests more efficiently.
    
26. **How can you improve security when using load balancers?**
    
    Improving security with load balancers can be achieved through a reverse proxy, which filters and controls traffic. You can also implement SSL encryption, use security groups, and apply web application firewalls (WAFs).
    
27. **Is it possible to implement SSL encryption when using a load balancer? If yes, then how?**  
    Yes, SSL encryption can be implemented with a load balancer. To do this, you configure SSL certificates on the load balancer, which allows it to encrypt traffic between clients and the load balancer and between the load balancer and backend servers.
    
28. **What is the purpose of sticky sessions when using a load balancer?**  
    Sticky sessions, or session affinity, ensure that a user's requests are consistently directed to the same server during their session. This is important for maintaining the session state and delivering a consistent user experience.
    
29. **Which Load Balancer provides advanced features, and why would you choose one over the other?**  
    Application Load Balancers (ALB) typically provide more advanced features than Network Load Balancers (NLB) due to their ability to operate at the application layer (Layer 7). ALBs offer features like content-based routing and are suitable for more complex application architectures. The choice depends on the specific requirements of your application.
    
30. **What is the difference between an internal and external Load Balancer?**  
    An internal Load Balancer is used for services intended for internal consumption within a Virtual Private Cloud (VPC) and does not route web traffic. An external Load Balancer, on the other hand, handles public-facing traffic.
    
31. **Can you explain what round-robin load balancing is?**  
    Round-robin load balancing is a method that evenly distributes traffic across multiple servers. Requests are sent to each server in a cyclic order, ensuring that each server gets a fair share of the incoming traffic.