\# 🛠️ Power of Math – Setup Guide



This guide explains how to deploy this serverless app on AWS.



---



\## Prerequisites



\- AWS account (Free Tier)

\- IAM user with Lambda, API Gateway, DynamoDB, and Amplify permissions

\- Python 3 installed

\- Git installed



---



\## Steps



\### 1. Deploy the Lambda Function

\- Go to AWS Lambda > Create Function

\- Runtime: Python 3.x

\- Paste the code from `lambda\_function.py`

\- Add permissions for DynamoDB

\- Set the environment variables if needed



\### 2. Create DynamoDB Table

\- Table name: `PowerOfMathDatabase`

\- Primary key: `ID` (String)



\### 3. Create API Gateway

\- Create a REST API

\- Method: POST

\- Link it to your Lambda function

\- Deploy to stage `dev`



\### 4. Update Frontend

\- In `index.html`, replace `"YOUR API GATEWAY ENDPOINT"` with your real API link

\- Test it locally



\### 5. Deploy Frontend with AWS Amplify

\- Push your code to GitHub

\- Connect repo to Amplify

\- Deploy and test



---



\## ✅ Done!

