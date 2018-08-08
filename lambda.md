# Lambda

## AWS Lambda

### Overview

* Fully-Managed serverless compute
* Event-driven execution
* Sub-second metering
* Multiple languages suppoted

Example
- Upload your code to AWS Lambda
- Set up your code to trigger from other AWS services, HTTP endpoints or in-app activity
- Lambda runs your code only when triggered using only the compute resources needed
- Pay just for the compute time you use

## Demostration
- Mobile app -> upload images to S3
- Install a function on Lambda to trigger uploaded images on S3 and recognite it, then return label of images

## Use cases
- Real-time image processing
    - Photograph is taken
    - Photo is uploaded to S3 Bucket
    - Lambda is triggered
    - Lambda runs image resizing code to generate web, mobile, and tablet sizes

- Extract, Transform, Load
    - Online order is placed
    - DynamoDB: Order data is stored in operational database
    - Lambda is triggered
    - Lambda runs data transformation code and loads results into data warehouse
    - Analytics generated from data

- IoT backends
    - Example: Sensors in Tractor detect need for a spare part and automatically place order
    - Tractor sensors send data to Kinesis
    - Lambda is triggered
    - Lambda runs code to detect trends in sensor data, identify anomadilies, and order replacements for faulty parts

- Mobile Backends
    - Example: Mobile backend for Social Media App
    - User posts status update
    - API GATEWAY: App makes REST API call to endpoint
    - Lambda is triggered
    - Lambda runs code to look up friends list and pushes status update notification to user's friends

- Web Backends
    - S3: Front-end code for weather app hosted in S3
    - User clicks link to get local weather information
    - API GATEWAY: App makes REST API call to endpoint
    - Lambda is triggered
    - Lambda runs code to retrieve local weather information and returns data back to user
  
## What is AWS Lambda
- AWS Lambda is a compute service that lets you run code without provisioning or managing servers. 
- AWS Lambda executes your code only when needed and scales automatically, from a few requests per day to thousands per second
- The Languages that AWS Lambda supports: Node.js, Java, C#, Go and Python

## When should I use AWS Lambda
- No servers to manage
- Continuous scaling
- Subsecond metering

# Lambda Functions
## Building Lambda Functions
- Authoring code for your Lambda function
    - Supporting Languages: 
        - Node.js – v8.10, v6.10 or v4.3
        - Java 8
        - Python 3.6 and 2.7
        - .NET Core – .NET Core 1.0.1, .NET Core 2.0 and .NET Core 2.1
        - Go 1.x
- Uploading code and creating Lambda functions
    - Creating a Deployment Package
        - Create a deployment package yourself
            - Create a .zip file consisting of your code and any dependencies
            - Need to set the appropriate security permissions for the zip package
            - You can upload your deployment package to S3, the package must reside in the same AWS region where you creating the Lambda function
        - Using Lambda console
            - When you create Lambda functions using the console, the console creates the deployment package for you, and then uploads it to create your Lambda function
    - Uploading a Deployment Package
        - Using Lambda Console or call API to create `Lambda Function`
        - Ref: [Create Function](https://docs.aws.amazon.com/lambda/latest/dg/API_CreateFunction.html)
    - Testing a Lambda Function
- Monitoring and troubleshooting
    - AWS Lambda automatically monitors functions on your behalf, reporting metrics through `Amazon CloudWatch`
