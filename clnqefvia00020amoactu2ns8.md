---
title: "AWS Architect Interview Q/A"
datePublished: Sat Oct 14 2023 18:56:55 GMT+0000 (Coordinated Universal Time)
cuid: clnqefvia00020amoactu2ns8
slug: aws-architect-interview-qa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1700671940549/1d1b79f1-7e3a-4685-b9a2-97e11a3157ec.png
tags: aws, amazon-web-services, aws-interview-question-and-answers, aws-solution-architect, aws-architect

---

1. **What is Cloud Computing? Can you talk about and compare any two popular Cloud Service Providers?**
    
    This question asks about cloud computing, which is the delivery of computing services over the Internet. It also requires a comparison of two popular cloud service providers, Amazon Web Services (AWS) and Microsoft Azure.
    
2. **You have some Private Servers on your premises, and you've distributed some workloads on the Public Cloud. What is this Architecture called?**
    
    This question is about a specific cloud architecture scenario where both private servers on-premises and public cloud resources are used. It asks for the name of this architecture, which is a "Hybrid Cloud."
    
3. **How do you choose an Availability Zone?**
    
    This question inquires about the factors to consider when selecting an Availability Zone within a cloud region, focusing on location, redundancy, cost, services, and compliance.
    
4. **You have a video transcoding application with a backlog. How do you efficiently add more instances temporarily?**
    
    This scenario-based question asks about the best method to handle a video transcoding backlog by efficiently adding instances. The answer suggests using an autoscaling group with a scale-out policy based on the queue size.
    
5. **When should you use Spot Instances, Reserved Instances, or On-Demand Instances for cost-effective operation?**
    
    This question involves understanding the pricing models for cloud instances and when to use each type, focusing on Spot Instances for cost-effective but variable workloads.
    
6. **Explain the difference between stopping and terminating an Amazon EC2 instance.**
    
    This question seeks to distinguish between stopping and terminating an Amazon EC2 instance, describing the impact on the instance, data, and associated costs.
    
7. **What does the command 'ec2-create-group CreateSecurityGroup' do concerning Amazon EC2 security groups?**
    
    This question is about an AWS CLI command and its purpose, which is to create a new security group in Amazon EC2.
    
8. **To run an instance on single-tenant hardware, what do you set the instance’s tenancy attribute to?**
    
    This question asks about setting the tenancy attribute to achieve single-tenant hardware, with the correct answer being "Dedicated."
    
9. **When do you incur costs with an Elastic IP Address (EIP)?**
    
    This question explores the situations in which costs are incurred for Elastic IP Addresses, explaining the conditions under which charges apply.
    
10. **Explain the differences between Spot Instances, On-Demand Instances, and Reserved Instances.**
    
    This question seeks to differentiate between Spot Instances, On-Demand Instances, and Reserved Instances in terms of pricing models and usage commitments.
    
11. **How is the processor state control feature used on the c4.8xlarge instance?**
    
    This question focuses on processor state control and its two states (C state and P state) in the context of a specific EC2 instance type (c4.8xlarge).
    
12. **Are Reserved Instances Available for Multi-AZ Deployments?**
    
    This question asks if Reserved Instances can be used in Multi-AZ Deployments, with the answer explaining their availability and usage.
    
13. **What network performance parameters can you expect when you launch instances in a cluster placement group?**
    
    This question inquires about the network performance when instances are launched in a cluster placement group, emphasizing low latency and high throughput.
    
14. **Which instance types can be used to deploy a 4-node cluster of Hadoop in AWS?**
    
    This question focuses on selecting appropriate EC2 instance types for a Hadoop cluster, considering the master and slave nodes and instance configuration.
    
15. **Where does an AMI fit into the architecture when designing a solution?**
    
    This question addresses the role of Amazon Machine Images (AMIs) in solution architecture, including their usage as templates for creating instances.
    
16. **Is one Elastic IP address enough for every instance that I have running?**
    
    This question asks if a single Elastic IP address is sufficient for all running instances and provides an explanation regarding EIP allocation.
    
17. **What are the best practices for security in Amazon EC2?**
    
    This question explores best practices for enhancing security in Amazon EC2 instances, covering aspects like AMIs, security updates, security groups, encryption, monitoring, and least privilege.
    

### Questions on Amazon Storage

1. **You need to configure an Amazon S3 bucket to serve static assets for your public-facing web application. Which method will ensure that all objects uploaded to the bucket are set to public read?**
    
    To ensure that all objects uploaded to an Amazon Simple Storage Service (S3) bucket are set to public read, you can use a bucket policy. A bucket policy is a JSON document that defines the access permissions for an S3 bucket. You can use a bucket policy to grant permissions to specific users or groups of users to perform specific actions on the objects in your bucket. To set all objects in your bucket to public read, you can use a specific bucket policy JSON configuration as described in the answer.
    
2. **Can S3 be used with EC2 instances, if yes, how?**
    
    Yes, Amazon Simple Storage Service (S3) can be used with Amazon Elastic Compute Cloud (EC2) instances. There are several ways to use S3 with EC2 instances, including storing and retrieving data, serving static assets for web applications, backing up data, and using S3 as a data source. To do this, you need to ensure that your EC2 instances have the appropriate permissions to access S3, typically by creating an IAM role and attaching it to your EC2 instances.
    
3. **A customer implemented AWS Storage Gateway with a gateway-cached volume at their main office. An event takes the link between the main and branch offices offline. Which methods will enable the branch office to access their data?**
    
    There are several methods to enable a branch office to access data stored in an AWS Storage Gateway with a gateway-cached volume when the link between the main and branch office is offline. These methods include using the local cache, enabling Amazon S3 Transfer Acceleration, setting up a VPN connection, or combining Transfer Acceleration with a VPN connection. The choice of method depends on the specific configuration and needs of the network infrastructure.
    
4. **A customer wants to leverage Amazon Simple Storage Service (S3) and Amazon Glacier as part of their backup and archive infrastructure. The customer plans to use third-party software to support this integration. Which approach will limit the access of the third-party software to only the Amazon S3 bucket named “company-backup”?**
    
    To limit the access of third-party software to only the Amazon S3 bucket named "company-backup," an Amazon Identity and Access Management (IAM) policy can be used. The IAM policy defines permissions for specific actions on resources. The provided IAM policy in the answer allows access to the "company-backup" bucket while denying access to other buckets.
    
5. **How can you speed up data transfer in Snowball?**
    
    You can speed up data transfer in Amazon Snowball by using multiple Snowballs to parallelize the transfer, enabling Amazon S3 Transfer Acceleration, using a faster network connection, choosing a larger Snowball appliance, or using a faster data transfer protocol like NFS or SMB.
    
6. **When you need to move data over long distances using the internet, for instance across countries or continents to your Amazon S3 bucket, which method or service will you use?**
    
    To move data over long distances using the internet to an Amazon S3 bucket, you can use Amazon S3 Transfer Acceleration. This feature utilizes Amazon CloudFront's global edge locations to accelerate data transfer, improving speed by up to 50% compared to standard internet transfers. You enable Transfer Acceleration for your S3 bucket and use the Transfer Acceleration endpoint when transferring data over long distances.
    
7. **When should I use a Classic Load Balancer and when should I use an Application load balancer?**
    
    You should use a Classic Load Balancer when you need basic load balancing with support for Transport Layer Security (TLS) offloading, and you should use an Application Load Balancer when you need advanced load balancing with support for containerized applications and microservices.
    
8. **What does Connection draining do?**
    
    Connection draining re-routes traffic from instances that are to be updated or have failed a health check. It is a service under Elastic Load Balancing (ELB) that constantly monitors the health of instances and ensures that traffic is directed away from unhealthy instances.
    
9. **When an instance is unhealthy, it is terminated and replaced with a new one, which of the following services does that?**
    
    Fault Tolerance. When Elastic Load Balancing (ELB) detects that an instance is unhealthy, it starts routing incoming traffic to other healthy instances in the region. If all instances in a region become unhealthy, and if you have instances in another availability zone/region, your traffic is directed to them.
    
10. **What are lifecycle hooks used for in AutoScaling?**
    
    They are used to put an additional wait time to a scale-in or scale-out event. Lifecycle hooks in Auto Scaling are used to add a wait time before any lifecycle action (launching or terminating an instance) occurs. This wait time can be used for various purposes, such as extracting log files before termination or installing necessary software before launching an instance.
    
11. **A user has set up an Auto Scaling group. Due to some issues, the group has failed to launch a single instance for more than 24 hours. What will happen to Auto Scaling in this condition?**
    
    Auto Scaling will suspend the scaling process. Auto Scaling allows you to suspend and then resume one or more of the Auto Scaling processes in your Auto Scaling group when you want to investigate a configuration problem or make changes without triggering the Auto Scaling process.
    
12. **To create a mirror image of your environment in another region for disaster recovery, which of the following AWS resources do not need to be recreated in the second region?**
    
    Route 53 Record Sets. Route 53 record sets are common assets that do not need to be replicated since Route 53 is valid across regions.
    
13. **A customer wants to capture all client connection information from his load balancer at an interval of 5 minutes, which of the following options should he choose for his application?**
    
    Enable AWS CloudTrail for the load balancer. AWS CloudTrail provides logging information for load balancers and other AWS resources, making it suitable for capturing connection information for analysis and security.
    
14. **A customer wants to track access to their Amazon Simple Storage Service (S3) buckets and use this information for internal security and access audits. Which of the following will meet the Customer's requirements?**
    
    Enable server access logging for all required Amazon S3 buckets. Server access logging for Amazon S3 buckets captures access information and is suitable for security and access auditing.
    
15. **Which of the following is true regarding AWS CloudTrail?**
    
    CloudTrail is enabled on a per-region and service basis, and logs can be delivered to a single Amazon S3 bucket for aggregation. CloudTrail is not enabled globally and may not cover all available services within a region.
    
16. **You have an EC2 Security Group with several running EC2 instances. You changed the Security Group rules to allow inbound traffic on a new port and protocol and then launched several new instances in the same Security Group. The new rules apply:**
    
    Immediately to all instances in the security group. Any rule specified in an EC2 Security Group applies immediately to all instances, regardless of when they were launched.
    
17. **What happens if CloudTrail is turned on for my account but my Amazon S3 bucket is not configured with the correct policy?**
    
    If CloudTrail is turned on for your AWS account but your Amazon S3 bucket is not configured with the correct policy, CloudTrail will not be able to deliver log files to the S3 bucket, and it may result in CloudTrail not recording API calls or generating errors.
    
18. **How do I transfer my existing domain name registration to Amazon Route 53 without disrupting my existing web traffic?**
    
    To transfer your domain to Amazon Route 53 without disrupting web traffic, follow these steps, including checking domain transfer eligibility, unlocking the domain, obtaining an authorization code, and initiating the transfer while keeping the DNS settings unchanged.
    
19. **Which of the following services you would not use to deploy an app?**
    
    AWS Lambda is not designed for deploying applications accessible to the public; it's primarily used for serverless event-driven functions.
    
20. **How is AWS Elastic Beanstalk different than AWS OpsWorks?**
    
    AWS Elastic Beanstalk is an application management platform that simplifies application deployment and scaling. AWS OpsWorks is a configuration management platform that offers more customization and control over infrastructure.
    
21. **What happens when one of the resources in a stack cannot be created successfully in AWS OpsWorks?**
    
    If one of the resources in an AWS OpsWorks stack cannot be created successfully, the stack creation process will fail, and OpsWorks will roll back changes, delete created resources, and provide the option to troubleshoot and resolve the issue.
    
22. **How does Elastic Beanstalk apply updates?**
    
    A. By having a duplicate ready with updates before swapping. Elastic Beanstalk prepares a duplicate copy of an instance before updating the original instance, routing traffic to the duplicate instance, and ensuring zero downtime during updates.
    
23. **How is AWS OpsWorks different than AWS CloudFormation?**
    
    AWS OpsWorks is a higher-level service focused on application management, while AWS CloudFormation is a lower-level service for infrastructure as code. OpsWorks provides integrated experiences for deployment, monitoring, and automation, while CloudFormation is for managing resources using templates.
    
24. **I created a key in the Oregon region to encrypt my data in the North Virginia region for security purposes. I added two users to the key and an external AWS account. I wanted to encrypt an object in S3, so when I tried, the key that I just created was not listed. What could be the reason?**
    
    The Key should be in the same region. The key created and the data to be encrypted should be in the same region for encryption to work correctly.
    
25. **What automation tools can you use to spin up servers?**
    
    Various automation tools can be used to spin up servers, including AWS CloudFormation, Ansible, Terraform, and Chef, among others. These tools allow you to automate the provisioning and management of server resources.
    
26. **A company needs to monitor the read-and-write IOPS for its AWS MySQL RDS instance and send real-time alerts to its operations team. Which AWS services can accomplish this?**
    
    Amazon CloudWatch can be used to monitor the performance of AWS resources, including RDS instances,