# Serverless Data Engineering

The goal of this project was to construct a serverless process flow using Amazon Lambda functions. Furthermore, this project also involved the integration of several different AWS services, including S3 (storage), DynamoDB (non-relational database), SQS (messaging), and Comprehend (natural language processing).

## Workflow

![image](https://user-images.githubusercontent.com/46541929/79709242-b3ff2b00-828f-11ea-9eaf-0fb28e587d38.png)

## Steps
1. Launch AWS Cloud9, create and configure settings for new environment
2. Create Github repo, create ssh keys, git clone
3. Create Serverless Application (Producer)
4. Create SQS Queue
5. Create table in DynamoDB
6. Deploy lambda function (Producer)
7. Verify deployment is successful in Lambda
8. Add Trigger to call lambda function every minute

![image](https://user-images.githubusercontent.com/46541929/79709968-9632c580-8291-11ea-8a25-85b5d767e3eb.png)

9. Trigger function is running and putting messages into SQS
10. Build Serverless Application (Consumer)
11. Install Required Packages then Deploy
12. Verify Deployment and Add SQS Trigger to pull 10 msg

![image](https://user-images.githubusercontent.com/46541929/79709979-9cc13d00-8291-11ea-8dc9-ba875cac73d9.png)

13. Observe Queue, CloudWatch Metrics, Logs

![image](https://user-images.githubusercontent.com/46541929/79709988-a054c400-8291-11ea-8962-540fa9a3bcf4.png)

14. Stores results in S3 Bucket

![image](https://user-images.githubusercontent.com/46541929/79709995-a5b20e80-8291-11ea-8916-f81361382e6c.png)

15. Download and review results (name, Wikipedia snippet, sentiment)

#### Demo and more hands-on overview of the serverless data engineering pipeline can be found here: https://youtu.be/eGFxhCXsOZQ
