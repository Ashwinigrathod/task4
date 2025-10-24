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
Deployment Steps

1. Open AWS Lambda Console

Go to Services → Lambda → Create function

Select Author from scratch

Name your function: helloLambda

Runtime: Python 3.9

Click Create function



2. Add Your Code

Paste the Python code above in the code editor.

Click Deploy



3. Add HTTP Trigger

Scroll to Function overview → Add trigger

Choose API Gateway

Select Create an API

API type: HTTP API

Security: Open

Click Add



4. Test the Function

Copy the API endpoint URL

Open it in a browser or Postman

✅ Expected Output:

Hello from my first AWS Lambda function!





---

🖼️ Screenshots

(Add your screenshots below)

✅ AWS Lambda function deployed successfully

🌐 Browser showing the “Hello” message



---

🌐 Function Endpoint

https://<your-api-id>.execute-api.<region>.amazonaws.com/


---

💬 How It Works

When someone visits the API URL, it sends an HTTP request to API Gateway.

The API Gateway triggers the Lambda function.

The function executes the Python code and returns a simple “Hello” message.

This setup demonstrates Function-as-a-Service (FaaS), where code runs without server management.



---

🧹 Clean Up Resources

After testing, delete your Lambda function to avoid unnecessary usage on your free AWS tier:

Go to AWS Lambda → Select your function → Delete



---

🧠 Key Learnings

Learned how serverless computing eliminates server management.

Understood the event-driven architecture of AWS Lambda.

Gained practical experience in deploying cloud functions.

Tested a live HTTP-triggered function using AWS API Gateway.



---

💡 Interview Prep Questions

1. What is serverless computing, and how does it differ from traditional hosting?


2. What are triggers in serverless functions?


3. What are cold starts, and why do they occur?


4. What are the main benefits of using FaaS like AWS Lambda?


5. How can you secure a Lambda HTTP endpoint?


6. Give one real-world example where serverless architecture is ideal.




---

🏁 Outcome

By completing this task, I successfully deployed a Python-based AWS Lambda function with an HTTP trigger using API Gateway.
This demonstrated my understanding of serverless architecture and how cloud functions can run automatically in response to events.


---

✨ Author

Ashwini Rathod
Cloud Computing Intern
📅 Task 4: Serverless Function Deployment
