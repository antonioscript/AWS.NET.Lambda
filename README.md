# AWS Lambda with .NET and DynamoDB

This project demonstrates how to create and publish a .NET application using **AWS Lambda** integrated with **Amazon DynamoDB**.

### Summary

- [Lambda](#Lambda)
- [API Gateway](#API-Gateway)
- [SQS](#SQS)
- [Test API](#Test-API)
- [NuGet Packages](#NuGet-Packages)

## Lambda

### Create Project Visual Studio

![image](https://github.com/user-attachments/assets/bc47ebca-ced9-4037-abe2-033be54604de)

![image](https://github.com/user-attachments/assets/ce9d9963-3591-4bf5-b4b9-442dddc04fc6)

![image](https://github.com/user-attachments/assets/366b44a9-0d38-427c-8c9b-0ea6be212f83)


### Publish to AWS Lambda

#### Steps to publish:

1. **Right-click the project** in Solution Explorer and select:

   **Publish to AWS Lambda**

   ![Publish to Lambda](https://github.com/user-attachments/assets/8b8a4b44-d25d-481f-9fc8-3cc5cb87a992)

2. **In the dialog that opens**, leave the default settings and click:

   **Next**

   ![Default settings](https://github.com/user-attachments/assets/7ab0ca42-3e6b-4120-84fb-9f9e50c85368)

3. **Choose an IAM Role** (or create a new one if needed), then click:

   **Upload**

   ![Choose IAM Role](https://github.com/user-attachments/assets/065e220d-f360-4a71-8c4d-3d639e473cb2)

4. Once uploaded, the Lambda function will appear in the AWS Console like this:

   ![Lambda in Console](https://github.com/user-attachments/assets/3feb43e0-462c-43c9-ab71-0f377d3db622)

   To test the function, simply click on **Test**:

   ![Test Lambda](https://github.com/user-attachments/assets/154c3726-a6ff-46e3-9bf2-6b7075017d03)

## API Gateway

1. **Create a route**

![image](https://github.com/user-attachments/assets/ef5e67bd-10e2-4439-a606-3243acdfea0c)

**2. Attach Integration**

![image](https://github.com/user-attachments/assets/e4477341-668b-437a-9a22-6c605fb4c87e)

3. **Choose Lambda Function to Integration type**

![image](https://github.com/user-attachments/assets/45206901-cd3f-431b-abc0-2513239d7fde)

4. **And choose the Lambda Function**

![image](https://github.com/user-attachments/assets/fe412ee0-2261-4edd-902e-80295b2ec65a)

5. **Result**

![image](https://github.com/user-attachments/assets/de36cbce-d971-4c1c-98e0-4adf05ec2da6)

![image](https://github.com/user-attachments/assets/ae4f22a2-fc59-4980-a84e-37a4fe6da6bc)

6. **Take endpoints**

**API Gateway**

Click on stateges and take on Invoke URL

![image](https://github.com/user-attachments/assets/c4b17eac-8b6f-490d-a225-dd58e2255d3c)


**Lambda**

Click on Triggers and Configuration

![image](https://github.com/user-attachments/assets/ac59b1c7-cd9d-44c4-81bc-1800423f98c7)


## SQS

### Create Project Visual Studio

![image](https://github.com/user-attachments/assets/7f1d643e-25b6-46a7-a993-01adffb5453e)


### Create Queue On Amazon Console 


![image](https://github.com/user-attachments/assets/e2d2a299-d194-47c6-bff8-92fd2cc725b4)

**Default Configuration**
![image](https://github.com/user-attachments/assets/0eed4215-7d19-473b-b7ee-b13b497c2866)

**Overview**
![image](https://github.com/user-attachments/assets/cfd7a919-95f1-4f95-b13f-310114002a9b)


### Add Trigger

![image](https://github.com/user-attachments/assets/523e0e36-0bf3-4f28-82dd-2a755bdcb382)**

**Choose source and configuration**

![image](https://github.com/user-attachments/assets/029cd987-5fe5-4995-aed2-7df69df9fff9)

**Overview**

![image](https://github.com/user-attachments/assets/a71f0b0f-61a7-41ed-ae71-a2e863293d7b)

### Test SQS

Go to SQS and click on 'Send and receibe messages'
![image](https://github.com/user-attachments/assets/a9d7c6e2-8664-4308-a831-d7842377ccf1)

## SNS

### Create Project Visual Studio

![image](https://github.com/user-attachments/assets/d144d388-f4e7-405d-ae05-5c51ed868916)


**Publish**

![image](https://github.com/user-attachments/assets/ff3f5a41-e4e0-4da7-b15e-0968a3fad4c7)


**Overview**

![image](https://github.com/user-attachments/assets/c9bfbfe8-fcc7-4f7d-8f04-9911a09f4093)


### Create SNS on Console

![image](https://github.com/user-attachments/assets/867bbfad-20b4-4779-882c-3c3d52d5fdcd)

**Create on default configuration**

![image](https://github.com/user-attachments/assets/9aff956f-d5fd-47bf-985c-b752df82a286)

**Overview**

![image](https://github.com/user-attachments/assets/4c0c0ebe-09d0-4242-b7a4-f8f8deb0fec6)


## Test API

1. **GET**
   
![image](https://github.com/user-attachments/assets/f243b6b3-9b97-4ae0-83c0-d6da8c165dec)


2. **POST**

![image](https://github.com/user-attachments/assets/07144606-7d6b-4c53-8365-ef2755193df6)



## NuGet Packages

- [AWSSDK.DynamoDBv2](https://www.nuget.org/packages/AWSSDK.DynamoDBv2)
- https://www.nuget.org/packages/Amazon.Lambda.APIGatewayEvents

