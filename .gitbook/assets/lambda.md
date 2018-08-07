# AWS Lambda
## Overview
- Fully-Managed serverless compute
- Event-driven execution
- Sub-second metering
- Multiple languages suppoted

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
- Uploading code and creating Lambda functions
- Monitoring and troubleshooting


