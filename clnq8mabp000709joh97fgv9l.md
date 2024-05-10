---
title: "AWS EventBridge Interview Q/A"
datePublished: Sat Oct 14 2023 16:13:57 GMT+0000 (Coordinated Universal Time)
cuid: clnq8mabp000709joh97fgv9l
slug: aws-eventbridge-interview-qa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1700674388905/7a6a3261-9d6c-4083-b23d-4209b8494f83.png
tags: cloud, aws, amazon-web-services, aws-interview-question-and-answers, aws-eventbridge

---

1. **What is Amazon EventBridge?**  
    Amazon EventBridge is a service that provides real-time access to changes in data in AWS services, your applications, and software as a service (SaaS) applications without the need to write code. You can choose an event source on the EventBridge console and then select a target from AWS services like AWS Lambda, Amazon Simple Notification Service (SNS), and Amazon Kinesis Data Firehose. EventBridge will automatically deliver events in near real-time.
    
2. **What are the steps for using Amazon EventBridge?**  
    To use Amazon EventBridge, you should choose an event source, which can be a partner SaaS application or an AWS service. You can do this by logging into your AWS account, accessing the EventBridge dashboard, and selecting the desired source. Ensure that your SaaS account is set up to emit events if you are using a partner application. Your event bus will be created automatically, and you can instrument your application with the AWS SDK to emit events to the event bus. You can also add a target for your events, like a Lambda function, and configure filtering rules.
    
3. **How can I get started using EventBridge?**  
    To get started with EventBridge, log in to your AWS account, go to the EventBridge console, and choose an event source from a list of partner SaaS applications and AWS services. Make sure your SaaS account is configured to emit events. EventBridge will create an event bus for you, and you can also use the AWS SDK to send events to your event bus. You can configure filtering rules and specify event targets, such as Lambda functions.
    
4. **What are EventBridge API Destinations?**  
    EventBridge API Destinations allow developers to control the throughput and authentication when sending events to on-premises or SaaS applications. EventBridge handles security and delivery, and you can set rules with input transformations to map event formats to the receiving service's format. When a rule is triggered, EventBridge transforms the event and sends it to the designated web service with authentication data. This eliminates the need for developers to create authentication components for the service.
    
5. **Can I publish my events to EventBridge?**  
    Yes, you can publish custom application-level events to EventBridge through the service's API operations. You can also set up scheduled events that occur periodically and process them using EventBridge-supported targets.
    
6. **How are CloudWatch Events related to Amazon EventBridge?**  
    Amazon EventBridge builds upon and extends CloudWatch Events. It uses the same API, endpoint, and infrastructure. Existing CloudWatch Events users can continue to use the same API and resources. EventBridge was introduced to expand the capabilities of CloudWatch Events for event-driven architectures.
    
7. **How do I secure access to EventBridge?**  
    EventBridge integrates with AWS Identity and Access Management (IAM) to allow users in your AWS account to specify which actions they can perform. IAM policies can be created to control permissions related to event buses and event targets.
    
8. **How does EventBridge relate to Amazon CloudWatch Events?**  
    EventBridge builds upon Amazon CloudWatch Events, using the same API and infrastructure. Existing CloudWatch Events users will experience no changes, and they can continue using the same resources and API.
    
9. **I currently use CloudWatch Events and want to try the features of EventBridge. Do I need to move my CloudWatch Events rules and permissions to EventBridge?** No, existing CloudWatch Events users can access their default bus, rules, and events in the new EventBridge console and API without the need to move rules and permissions.
    
10. **Which AWS services are included with Amazon EventBridge as event sources?** Amazon EventBridge supports over 90 AWS services as event sources, including AWS Lambda, Amazon Kinesis, AWS Fargate, and Amazon Simple Storage Service (S3).
    
11. **I'm already using CloudWatch Events and don't need the features of EventBridge. What will change for me?**  
    If you're already using CloudWatch Events and don't require the additional features of EventBridge, nothing will change for you. You can continue to use CloudWatch Events as before.
    
12. **Are you going to phase out CloudWatch Events one day?**  
    No, CloudWatch Events is not being deprecated. EventBridge builds upon CloudWatch Events and introduces new features. Over time, the name "Amazon CloudWatch Events" may be replaced with "Amazon EventBridge."
    
13. **Which AWS services are integrated as event sources for Amazon EventBridge?** Amazon EventBridge supports over 90 AWS services as event sources, including AWS Lambda, Amazon Kinesis, AWS Fargate, and Amazon Simple Storage Service (S3). A full list of integrations can be found in the EventBridge documentation.
    
14. **Which AWS services are integrated as event targets for EventBridge?** EventBridge supports over 15 AWS services as event targets, including Lambda, Amazon Simple Queue Service (SQS), Amazon SNS, Amazon Kinesis Streams, and Kinesis Data Firehose. A complete list of integrations can be found in the EventBridge documentation.
    
15. **What are EventBridge Archive and Replay Events?**  
    Event Replay is a feature in EventBridge that allows you to reprocess past events to an event bus or a specific EventBridge rule. This feature aids in debugging applications, extending them by using historic events, and recovering from errors.
    
16. **Does the Serverless Application Model (AWS SAM) allow for the use of schema?**  
    Yes, you can build serverless apps on EventBridge with schema using the AWS SAM CLI's interactive mode. This allows you to create applications with Lambda functions and code for handling events with a specific schema. This simplifies the development process and enhances code validation and auto-complete.
    
17. **How can writing less code using the schema registry benefit me?**  
    Writing less code is made possible by utilizing the schema registry, which automatically identifies event schemas and generates code bindings. This eliminates the need for manual event schema management, deserialization, and validation, making development more efficient.
    
18. **What are EventBridge API Destinations?**  
    EventBridge API Destinations allow for controlled event throughput and authentication when sending events to on-premises or SaaS applications. Rules with input transformations map event formats to the receiving service, and EventBridge handles security and delivery, eliminating the need to create authentication components.