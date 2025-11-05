Exercise 6: Sending an Email using Amazon SNS (Simple Notification Service)

This project demonstrates how to send email notifications using **Amazon SNS (Simple Notification Service)**.  
It was completed as part of my **Cloud Architecture practicals** for the 5th semester of **BCA (Cloud Computing)** at **Kristu Jayanti College**

Objective

To understand and implement **Amazon SNS** for sending email notifications by:
- Creating an SNS topic  
- Subscribing an email endpoint  
- Publishing a message through the SNS topic  

---

Steps Performed

Step 1: Open SNS Console
- Logged in to **AWS Management Console**
- Searched for **SNS (Simple Notification Service)**

Step 2: Create a Topic
- Navigated to **Topics → Create Topic**
- Chose **Standard type**
- Gave the topic a name (e.g., `BCATESTEMAIL`)
- Clicked **Create topic**

Step 3: Subscribe an Email Address
- Opened the created topic → **Create subscription**
- **Protocol:** Email  
- **Endpoint:** Entered email address (e.g., `yourname@gmail.com`)
- Clicked **Create subscription**
- Confirmed the subscription from the confirmation email sent by AWS

Step 4: Publish a Message
- On the topic page → Clicked "Publish message"
- Entered:
  - Subject: AWS SNS Email Test  
  - Message body: “This is a test message from AWS SNS”
- Clicked Publish message

Result: The email was successfully sent to all subscribed email addresses.


AWS Services Used
- Amazon SNS – for creating topics, subscriptions, and sending messages  
- IAM – for basic permissions  
- AWS Management Console – for configuration and testing  

Output
- Received email notification:  

