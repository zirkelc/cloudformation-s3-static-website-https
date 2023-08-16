# CloudFormation Template for Static Website Hosting 
This repository contains the CloudFormation template for the static website hosting on AWS with support for HTTPS and a custom domain name.

It can be deployed via [CloudFormation console](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-console-create-stack.html) or the [AWS CLI](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-cli-creating-stack.html). 

It creates the following resources:
* S3 bucket for the website content
* CloudFront distribution for HTTPS support
* Route53 record for the custom domain name

Please refer to my [blog post](https://dev.to/zirkelc/aws-website-hosting-s3-https-cloudfront-route53-4j4-temp-slug-5410438) for more details.
