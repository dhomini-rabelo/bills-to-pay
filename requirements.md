# Bills-to-pay

## Features

- [ ] It should be possible to register Workers.
- [ ] It should be possible to authenticate with a Worker.
- [ ] It should be possible to register, remove Payments.
- [ ] It should be possible to configure a worker's notification options.


## Development requirements

- [ ] Deployment must be done on an ec2.
- [ ] The ec2 will have a policy to access the lambda.
- [ ] Data will be saved in dynamoDB.
- [ ] SQS as a queue for sending notifications.
- [ ] We will have a lambda that will be executed once a day, to send the SQS the notifications that need to be sent.
- [ ] SQS and SNS will be used to send the notifications.
- [ ] Authentication will be provided by Cognito.


## Business rules

- [ ] The worker will always receive a notification whenever an account is.
between the day of issue and the due date, if the bill has not yet been paid or received.
- [ ] The worker can choose whether to receive notification by SMS or email.
- [ ] When registering an account, it can inform whether it has already been paid in the current month.
