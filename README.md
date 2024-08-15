# AWS-ShellScript
Latest project for beginners to master Shell script and aws
Here’s a simple README file for your project:

---

# AWS Resource Listing Script

This script helps you list various resources in your AWS account, such as EC2 instances, S3 buckets, RDS instances, and more. The script uses the AWS CLI to query and display resources for a specified service in a given region.

## Features

The script currently supports listing resources for the following AWS services:

- EC2
- S3
- RDS
- Lambda
- EBS
- SQS
- ELB
- SNS
- VPC
- IAM
- DynamoDB
- Route53
- CloudFormation

## Prerequisites

- **AWS CLI**: Ensure that the AWS CLI is installed and configured on your system.
- **AWS Configuration**: You must have your AWS CLI configured with valid credentials (via `aws configure`).

## Usage

To run the script, use the following command:

```bash
./aws_resource_list.sh <aws_region> <aws_service>
```

### Example:

```bash
./aws_resource_list.sh us-east-1 ec2
```

This example will list all EC2 instances in the `us-east-1` region.

## Arguments

1. `<aws_region>`: The AWS region where you want to list resources (e.g., `us-west-2`, `eu-central-1`).
2. `<aws_service>`: The service for which you want to list resources. Supported values include:

    - `ec2`
    - `s3`
    - `rds`
    - `lambda`
    - `ebs`
    - `sqs`
    - `sns`
    - `vpc`
    - `iam`
    - `dynamodb`
    - `route53`
    - `cloudformation`
    - `cloudwatch`
    - `cloudfront`

## Error Handling

The script checks for:

- **AWS CLI installation**: If the CLI is not installed, you’ll receive an error message.
- **AWS CLI configuration**: If the CLI is not configured, the script will prompt you to configure it.

## Example Outputs

- Listing EC2 Instances:
    ```bash
    Listing EC2 Instances in us-east-1
    ```
- Listing S3 Buckets:
    ```bash
    Listing S3 Buckets in us-east-1
    ```

## Troubleshooting

- **Invalid Service Name**: If you provide an unsupported service name, the script will notify you and exit.
- **Missing Arguments**: The script requires both the region and service name to run. If any are missing, it will show usage instructions.

## Author

**Shuaib**  
Version: v1

