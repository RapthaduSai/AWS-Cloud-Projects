 Exercise 7: Invoking an AWS Lambda Function

This project demonstrates how to create, deploy, and invoke an AWS Lambda function using the AWS Management Console and **Lambda Function URL.  
It was completed as part of my Cloud Architecture Practicals for the 5ᵗʰ semester of BCA (Cloud Computing) at Kristu Jayanti College.


  Objective
To understand **serverless computing** using AWS Lambda by:
- Creating a Lambda function
- Writing a simple Python function
- Invoking the function using a public Function URL


  Steps Performed

   1.Create a Lambda Function
- Logged in to **AWS Management Console**
- Navigated to **Lambda → Create function**
- Selected:
  - Author from scratch
  - Function name: `helloFunction`
  - Runtime: Python 3.x
  - Permissions: Default execution role


   2.Add Lambda Function Code
Replaced the default code with the following Python code:

```python
import json

def lambda_handler(event, context):
    return {
        "statusCode": 200,
        "headers": { "Content-Type": "application/json" },
        "body": json.dumps({ "message": "Hello from Lambda!" })
    }
