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






