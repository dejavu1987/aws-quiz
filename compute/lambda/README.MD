# AWS Lambda

## Features of AWS Lambda

Which of the following are features of Lambda? (Select FOUR.)

- [x] You can run code without provisioning or managing servers.
- [x] It initiates functions on your behalf in response to events.
- [ ] You don't need to configure memory or CPU.
- [x] It scales automatically.
- [x] It provides built-in monitoring and logging.
- [ ] You can update the operating system dynamically.

#### Explanation

AWS Lambda allows you to run code without managing servers, initiates functions in response to events, scales automatically, and provides built-in monitoring and logging. Memory configuration is required, but CPU and OS updates are handled by AWS.

## Invocation Models in AWS Lambda

Which statements about invocation models are correct? (Select THREE.)

- [x] Amazon S3 triggers Lambda via an asynchronous push.
- [x] Amazon API Gateway triggers Lambda synchronously.
- [ ] When Alexa is the event source, Lambda will make three attempts to invoke the function before putting the failed invocation into the dead letter queue (DLQ).
- [ ] DynamoDB must have an execution role to invoke Lambda.
- [x] Amazon SQS triggers Lambda via the polling invocation model.

#### Explanation

Correct! Amazon S3 and Amazon API Gateway use asynchronous and synchronous push models, respectively. For Alexa, there are no automatic retries, and DynamoDB does not require an execution role for invoking Lambda. Amazon SQS uses the polling invocation model for triggering Lambda.


## IAM Entities for Lambda Function Interaction

What IAM entities must be included in an execution role for a Lambda function to interact with other services, such as DynamoDB? (Select TWO.)

- [x] IAM policy that defines the actions that can be taken within DynamoDB
- [x] Trust policy that grants "AssumeRole" permission to Lambda to act on DynamoDB
- [ ] IAM group defining users of the Lambda function
- [ ] IAM user with admin permissions to Lambda and DynamoDB

#### Explanation

You need both the IAM policy that defines the actions Lambda can take and a trust policy that grants Lambda the "AssumeRole" permission. You do not have to create any IAM users or groups to allow Lambda to take action.

---

## Resource Policy in AWS Lambda

Which of these statements describe a resource policy? (Select THREE.)

- [ ] Must be chosen or created when you create a Lambda function
- [x] Can give Amazon S3 permission to initiate a Lambda function
- [ ] Can give Lambda permission to write data to a DynamoDB table
- [x] Can grant access to the Lambda function across AWS accounts
- [x] Determines who has access to invoke the function
- [ ] Determines what Lambda is allowed to do

#### Explanation

Correct! A resource policy determines who can initiate your function (e.g., Amazon S3), grants access across accounts, and controls who has access to invoke the function. It is not chosen or created when creating a Lambda function and does not specify what Lambda is allowed to do; that is controlled by the execution role's IAM policy.

## Match Lambda Function Terms to Definitions


| Lambda Function Terms      | Definitions                                               |
| -------------------------- | --------------------------------------------------------- |
| Handler method             | An entry point that AWS Lambda calls to initiate your Lambda function |
| Context object             | This is generated by AWS and provides metadata about the action |
| Event object               | An object with information about the event that initiated the Lambda function |

#### Explanation

The handler method is the entry point to your Lambda function. The event object provides information about the event that initiated the Lambda function. The context object is generated by AWS and provides metadata about the execution.



## AWS Lambda Authoring using AWS Management Console

What is the best purpose for authoring using the AWS Management Console?

- [ ] Small standalone applications less than 10 MB package
- [x] Simple one-function applications with no custom libraries and experimentation
- [ ] Packages greater than 10 MB or part of continuous integration and continuous delivery (CI/CD) managed applications

#### Explanation

That's correct! The Lambda management console is best for simple functions with no custom libraries and is a great way to start experimenting with Lambda.

## Match Items to Descriptions

Drag the items in the left column to the correct items on the right column.

| Items                  | Descriptions                                             |
| ---------------------- | -------------------------------------------------------- |
| CloudFormation Template | Like a house blueprint – you can treat infrastructure as code |
| AWS SAM Template        | Streamlined CloudFormation Template for serverless applications |
| AWS SAM CLI             | Tool for local testing and debugging of serverless applications |
| Deploy                 | AWS SAM CLI command for deploying AWS SAM template       |


## Troubleshooting Lambda Function Duration

A developer has been asked to troubleshoot a Lambda function that is in production. They've been told that it runs for 5 minutes and has been asked to reduce its duration to save on billable costs. Which actions should the developer take? (Select THREE.)

- [ ] Test the function from the console once to confirm that it is taking 5 minutes.
- [x] Confirm whether 5 minutes is the typical duration through production monitoring.
- [ ] Decrease the timeout to 4 minutes.
- [x] Test at higher memory configurations and compare the duration and cost at each configuration.
- [x] Check whether any unnecessary SDK components are in the deployment package.

#### Explanation

A developer must make sure that a 5-minute duration isn't reflective of a single invocation. Instead of running it once from the console, they need to examine how it actually runs in production. Decreasing the timeout would save costs, but it would probably mean that the function would frequently fail to complete. A best practice is to experiment with different memory configurations and estimate whether a higher memory configuration would actually be less expensive. They can also determine whether there are unnecessary components in the function itself that could be removed to speed up its initialization.


## Setting Concurrency Limit on Lambda Function

What are some reasons a developer would set a concurrency limit (or reserve) on a function? (Select THREE.)

- [x] Manage costs
- [x] Regulate how long it takes to process a batch of events
- [x] Match the limit with a downstream resource
- [ ] Help CloudWatch track logging events
- [ ] Ensure that Amazon Simple Queue Service (Amazon SQS) queues are cleared efficiently
- [ ] Limit the memory that is used

#### Explanation

Setting a concurrency limit helps manage costs, regulate the processing time for a batch of events, and match the limit with a downstream resource. It is not used to help CloudWatch track logging events, ensure efficient clearing of Amazon SQS queues, or limit memory usage.


## Lambda Function Versioning

Which statements are true? (Select THREE.)

- [x] When you create a Lambda function, only one version exists: the $LATEST version.
- [ ] Versioning is a requirement for your Lambda functions.
- [ ] You can specify a versioning number scheme that Lambda will use.
- [x] You can reference any version with an alias.
- [x] You can reference a version or an alias in the Amazon Resource Name (ARN).

#### Explanation

Correct! When you create a Lambda function, only one version exists: the $LATEST version. Versioning is not a requirement for Lambda functions, and you cannot specify a versioning number scheme. You can reference any version with an alias, and you can reference a version or an alias in the Amazon Resource Name (ARN).

## Task Matching with AWS Tools

Match the task to the tool you would use to perform it.

| Task                                                                       | Tool                  |
| -------------------------------------------------------------------------- | --------------------- |
| Review metrics on invocations, errors, and throttling for a Lambda function | Amazon CloudWatch     |
| Manually review errors for Lambda invocations that failed and must be addressed | Dead-letter queue   |
| Review trace details about an invocation to identify potential bottlenecks   | AWS X-Ray             |
| Audit actions made against your applications                                | AWS CloudTrail        |

#### Explanation

Correct! Amazon CloudWatch provides metrics for Lambda functions, dead-letter queues are used to manually review errors, AWS X-Ray is used to review trace details, and AWS CloudTrail is used to audit actions made against your applications.

