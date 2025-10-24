# task4
# ☁️ Cloud Internship – Task 4  
## 🚀 Deploy a Serverless Function to the Cloud  
### 👩‍💻 By: *Ashwini G Rathod*

---

## 🎯 Objective
To understand *serverless computing* by creating and deploying a simple *cloud function (FaaS)* that executes automatically when triggered — without managing any servers.

This task demonstrates *event-driven computing, **resource optimization, and **cost-effective deployment* in a modern cloud environment.

---

## 🧰 Tools & Technologies Used
- *AWS Lambda* (Free Tier)
- *AWS API Gateway* (for HTTP trigger)
- *Python 3.9*
- *AWS Management Console*

---

## 🧠 What is a Serverless Function?
A *serverless function* allows developers to run code in the cloud without provisioning or managing servers.  
It executes in response to specific events, such as:
- HTTP requests  
- File uploads (S3)  
- Database changes  

The cloud provider automatically handles scaling, monitoring, and availability.

---

## 🪄 Function Code (main.py)

```python
import json

def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'headers': {
            'Content-Type': 'text/plain'
        },
        'body': 'Hello from my first AWS Lambda function!'
    }
