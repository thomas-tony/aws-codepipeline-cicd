# AWS CodePipeline CI/CD

This project demonstrates setting up a CI/CD pipeline using AWS CodePipeline.

## Prerequisites

- AWS Account
- AWS CLI configured
- GitHub account

## Project Structure

- `src/`: Application source code
- `infrastructure/`: CloudFormation template for AWS resources
- `buildspec.yml`: Build specification file for CodeBuild

## Setup Instructions

1. Clone the repository.
2. Update the `infrastructure/template.yaml` file with your AWS account details.
3. Deploy the CloudFormation stack.
4. Commit and push changes to the CodeCommit repository.

## Deploying the Stack

```sh
aws cloudformation deploy --template-file infrastructure/template.yaml --stack-name my-codepipeline-stack --capabilities CAPABILITY_NAMED_IAM
```

## Testing the Pipeline

1. Make changes to the source code in the src/ directory.
2. Commit and push changes to trigger the pipeline.

