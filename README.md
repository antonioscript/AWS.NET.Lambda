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

**Create a route**
![image](https://github.com/user-attachments/assets/ef5e67bd-10e2-4439-a606-3243acdfea0c)


## NuGet Packages

To enable interaction between your Lambda function and DynamoDB, install the following NuGet package:

- [AWSSDK.DynamoDBv2](https://www.nuget.org/packages/AWSSDK.DynamoDBv2)

You can install it via the NuGet Package Manager or using the CLI:

```bash
dotnet add package AWSSDK.DynamoDBv2
