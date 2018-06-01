# Prerequisites

## AWS 

This tutorial leverages the [AWS Cloud](https://aws.amazon.com/console) to streamline provisioning of the compute infrastructure required to bootstrap a Kubernetes cluster from the ground up. [Sign up](https://portal.aws.amazon.com/billing/signup#/start) for the free tier period.

[Estimated cost](https://calculator.s3.amazonaws.com/index.html#r=IAD&key=calc-CAF3CFD3-C091-4FBB-B889-98A98CEAF1C0) to run this tutorial.

> The compute resources required for this tutorial exceed the AWS Free tier quota.

## AWS CLi

### Install AWS CLI

Follow the AWS Cli Getting Started Guide [documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html) to install and configure the `aws` command line utility.

Verify the AWS Cli version is 1.14 or higher:

```
aws --version
```
The output shoud be similar to 
```
aws-cli/1.14.10 Python/3.6.5 Darwin/17.4.0 botocore/1.8.14
```
### Configure AWS Cli 

You must configure aws cli to proceed with this tutorial. Please refer to the
configuration guide [documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html)

If everything is ok, you type the following command: 
```
aws ec2 describe-regions
```

And get the output:
```
{
    "Regions": [
        {
            "Endpoint": "ec2.ap-south-1.amazonaws.com",
            "RegionName": "ap-south-1"
        },
        {
            "Endpoint": "ec2.eu-west-3.amazonaws.com",
            "RegionName": "eu-west-3"
        },
        {
            "Endpoint": "ec2.eu-west-2.amazonaws.com",
            "RegionName": "eu-west-2"
        },
        {
            "Endpoint": "ec2.eu-west-1.amazonaws.com",
            "RegionName": "eu-west-1"
        },
        {
            "Endpoint": "ec2.ap-northeast-2.amazonaws.com",
            "RegionName": "ap-northeast-2"
        },
        {
            "Endpoint": "ec2.ap-northeast-1.amazonaws.com",
            "RegionName": "ap-northeast-1"
        },
        {
            "Endpoint": "ec2.sa-east-1.amazonaws.com",
            "RegionName": "sa-east-1"
        },
        {
            "Endpoint": "ec2.ca-central-1.amazonaws.com",
            "RegionName": "ca-central-1"
        },
        {
            "Endpoint": "ec2.ap-southeast-1.amazonaws.com",
            "RegionName": "ap-southeast-1"
        },
        {
            "Endpoint": "ec2.ap-southeast-2.amazonaws.com",
            "RegionName": "ap-southeast-2"
        },
        {
            "Endpoint": "ec2.eu-central-1.amazonaws.com",
            "RegionName": "eu-central-1"
        },
        {
            "Endpoint": "ec2.us-east-1.amazonaws.com",
            "RegionName": "us-east-1"
        },
        {
            "Endpoint": "ec2.us-east-2.amazonaws.com",
            "RegionName": "us-east-2"
        },
        {
            "Endpoint": "ec2.us-west-1.amazonaws.com",
            "RegionName": "us-west-1"
        },
        {
            "Endpoint": "ec2.us-west-2.amazonaws.com",
            "RegionName": "us-west-2"
        }
    ]
}
```


Next: [Installing the Client Tools](02-client-tools.md)