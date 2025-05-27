# AWS Lambda with .NET and DynamoDB

This project demonstrates how to create and publish a .NET application using **AWS Lambda** integrated with **Amazon DynamoDB**.

## Publish to AWS Lambda

### Steps to publish:

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


## Test API

1. **GET**
   
![image](https://github.com/user-attachments/assets/f243b6b3-9b97-4ae0-83c0-d6da8c165dec)


2. **POST**

![image](https://github.com/user-attachments/assets/07144606-7d6b-4c53-8365-ef2755193df6)



## NuGet Packages

- [AWSSDK.DynamoDBv2](https://www.nuget.org/packages/AWSSDK.DynamoDBv2)
- https://www.nuget.org/packages/Amazon.Lambda.APIGatewayEvents

