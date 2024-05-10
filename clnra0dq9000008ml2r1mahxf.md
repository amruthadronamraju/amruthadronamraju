---
title: "AWS SNS Interview Q/A"
datePublished: Sun Oct 15 2023 09:40:40 GMT+0000 (Coordinated Universal Time)
cuid: clnra0dq9000008ml2r1mahxf
slug: aws-sns-interview-qa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1700669362531/97050969-f4c2-4525-8274-351b7c91c538.png
tags: aws, amazon-web-services, amazon-sns, aws-interview-question-and-answers, aws-sns

---

1. **What is AWS SNS?**
    
    AWS SNS, or Amazon Simple Notification Service, is a fully managed messaging service within Amazon Web Services (AWS). It enables users to send messages to multiple recipients or devices in a flexible and scalable manner. SNS supports various messaging protocols, including SMS, email, and HTTP, and can deliver messages to a wide range of endpoints, such as mobile phones, email addresses, and web applications. It's used for one-to-many messaging and building event-driven architectures.
    
2. **How does AWS SNS work?**
    
    AWS SNS works by allowing users to create topics, subscribe endpoints to these topics (e.g., email addresses, mobile phone numbers), and then publish messages to these topics. When a message is published to a topic, SNS automatically delivers the message to all subscribed endpoints. The endpoints process the messages according to their logic, which could include sending an email or an SMS.
    
3. **What are the benefits of Amazon SNS?**
    
    Amazon SNS offers several benefits, including high reliability with messages stored across AWS regions, automatic scalability for handling varying workloads, message filtering for targeted message delivery, and strong security measures to control who can publish or subscribe to topics. SNS also supports message encryption and private message publishing.
    
4. **How to Create an Amazon SNS Topic?**
    
    To create an Amazon SNS topic, you need to access the AWS Management Console, navigate to the Amazon SNS dashboard, click "Create a topic," provide a name and display name for the topic, and confirm the creation. You can also programmatically create topics using AWS SDKs or the SNS API.
    
5. **How to Set Filter Policies for the SNS Subscriptions?**
    
    Filter policies for SNS subscriptions can be set through the AWS Management Console by navigating to the SNS dashboard, selecting the topic with the subscription you want to modify, clicking "Subscriptions," editing the subscription, and entering a JSON object in the "Filter policy" field to define the filtering criteria.
    
6. **How much does it cost to send 1 million messages through SNS?**
    
    The cost of sending 1 million messages through Amazon SNS varies depending on the messaging protocol used and the number of endpoints subscribed to your topics. For instance, in the US East (N. Virginia) region, it may cost $0.75 for SMS, $0.10 for email, and $0.40 for HTTP/HTTPS. These prices can vary based on region and usage beyond the free tier.
    
7. **What is the difference between direct and fanout messaging models? Which one is preferred in which situations?**
    
    Amazon SNS supports direct messaging where a message is sent to specific recipients and fanout messaging where a message is broadcast to all subscribers of a topic. The choice between them depends on your use case. Direct messaging is suitable when you want to send a message to a specific group of recipients. Fanout messaging is preferred when you want to broadcast a message to a large number of recipients without specifying them individually.
    
8. **Why isn’t AWS SNS used more extensively than other pub/sub mechanisms like Kafka or RabbitMQ?**
    
    While AWS SNS is widely used, it may not be as extensively used as other pub/sub mechanisms like Kafka or RabbitMQ in certain scenarios due to factors like its simplicity for event-based messaging, language support, tight integration with other AWS services, and cost considerations. More complex event processing or specific language support needs might lead to choosing alternative pub/sub mechanisms.
    
9. **Can you explain the Architecture of AWS SNS?**
    
    The architecture of AWS SNS consists of Publishers (components or applications that send messages to SNS topics), Topics (channels for sending and receiving messages), Subscribers (components or applications that receive messages), and Notifications (messages sent by publishers and received by subscribers). SNS supports various messaging protocols and can be used for both direct and fanout messaging, allowing flexible and scalable message distribution.
    
10. **Do all subscribers receive the same message at the same time? Or is there a delay between messages being received by different subscribers?**
    
    In Amazon SNS, all subscribers of a topic receive the same message, but there may be a delay between when the message is received by different subscribers. The delay can vary due to factors such as the messaging medium, subscriber locations, and message processing. SNS aims to deliver messages as quickly as possible to all subscribers but does not guarantee exact simultaneous delivery.
    
11. **What are some common use cases for SNS?**
    
    This question asks about the various scenarios in which Amazon Simple Notification Service (SNS) can be used. The answer lists common use cases, including mobile push notifications, email notifications, event-driven notifications, message fan-out, and alerts and notifications.
    
12. **How can you subscribe to an SNS topic without using email or SMS as a medium?**
    
    This question is about subscribing to an SNS topic using messaging protocols other than email or SMS. The answer explains how you can use protocols like HTTP/HTTPS, AWS Lambda, and the Application protocol to subscribe to an SNS topic.
    
13. **Is there any limit on the number of messages sent per second by SNS? If yes, then what are they?**
    
    This question inquires about the limitations on message throughput in Amazon SNS. The answer provides details on the message-per-second limits for various messaging protocols, such as SMS, email, HTTP/HTTPS, and application messages.
    
14. **Are SNS topics durable? If yes, why?**
    
    This question asks whether SNS topics are durable and why. The answer explains that SNS topics are durable because they use Amazon Simple Queue Service (SQS) to store undelivered messages, ensuring message persistence.
    
15. **What is the best way to configure SNS for high availability?**
    
    This question seeks advice on configuring SNS for high availability. The answer outlines best practices, such as using multiple regions, protocols, endpoints, and Amazon CloudWatch alarms.
    
16. **Is it possible to disable SNS notifications once they have been enabled? If yes, then how?**
    
    This question explores the possibility of disabling SNS notifications and how to do it. The answer explains that you can disable SNS notifications by unsubscribing from the SNS topic or by deleting the subscription.
    
17. **How do you create a topic in SNS?**
    
    This question asks about the process of creating a topic in Amazon SNS. The answer provides the steps for creating an SNS topic using the AWS Management Console.
    
18. **How do you subscribe to an SNS topic?**
    
    This question is about subscribing to an SNS topic. The answer outlines the steps to subscribe to an SNS topic using the AWS Management Console.
    
19. **How do you send a message to an SNS topic?**
    
    This question seeks information on how to send a message to an SNS topic. The answer provides the steps for publishing a message to an SNS topic using the AWS Management Console.
    
20. **Does SNS support content filtering? If yes, how?**
    
    This question asks if SNS supports content filtering and how it can be implemented. The answer explains that SNS supports content filtering through filter policies and provides steps to create such policies.
    
21. **What does it mean when we say that SNS notifications are decoupled from the publish-subscribe mechanism?**
    
    This question inquires about the concept of decoupling in SNS. The answer clarifies that SNS notifications are decoupled from the publisher and subscriber, and it elaborates on the benefits of this decoupling.
    
22. **Can you give me some examples of real-world applications that use SNS?**
    
    This question asks for real-world applications that utilize SNS. The answer provides examples, such as mobile push notifications, email marketing, monitoring and alerts, microservices, and social media applications.
    
23. **What is the maximum size of an SNS notification payload?**
    
    This question seeks information about the maximum payload size in SNS notifications. The answer provides the maximum payload sizes for various messaging protocols.
    
24. **Are messages delivered in the order that they were published? If not, then how do you ensure that messages are delivered in the correct sequence?**
    
    This question addresses message delivery orders in SNS. The answer explains that SNS does not guarantee message ordering and suggests approaches to ensure correct sequencing.
    
25. **How to Publish Messages to the Topic?**
    
    This question is about publishing messages on an SNS topic. The answer provides steps for publishing messages using the AWS Management Console.
    
26. **How to Verify Your AWS SNS Message Deliveries?**
    
    This question asks about verifying message deliveries in SNS. The answer outlines the steps to verify message deliveries and check the delivery status of subscriptions.