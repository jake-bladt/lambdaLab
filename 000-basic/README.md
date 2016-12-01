# Basic AWS Lambda

This exercise requires the AWS CLI, which is kludgy on Windows. So, I'm creating a docker container to run the aws-cli.

From the dockerhub documentation:

```docker run --rm -e AWS_ACCESS_KEY_ID=my-key-id -e AWS_SECRET_ACCESS_KEY=my-secret-access-key -v $(pwd):/aws mikesir87/aws-cli aws ecs register-task-definition --cli-input-json file://aws/task-definition.json```
