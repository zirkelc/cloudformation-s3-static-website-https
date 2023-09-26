# CloudFormation Template for Static Website Hosting 
This repository contains the CloudFormation template for the static website hosting on AWS with support for HTTPS and a custom domain name.

It can be deployed via [CloudFormation console](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-console-create-stack.html) or the [AWS CLI](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-cli-creating-stack.html). 

It requires the following inputs:
* ARN of an existing [ACM certificate](https://docs.aws.amazon.com/acm/latest/userguide/gs-acm-request-public.html)
* Name of an existing [Route53 domain](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-configuring.html)
* Name of the new S3 bucket that hosts the website

It creates the following resources:
* S3 bucket for the website content
* CloudFront distribution for HTTPS support
* Route53 record for the custom domain name

There are two templates in this repository:
* `templates/classic.yml` - uses a public S3 bucket **with** static website hosting
* `templates/modern.yml` - uses a private S3 bucket **without** static website hosting

Please refer to my [blog series](https://dev.to/zirkelc/series/24194) for more details.
