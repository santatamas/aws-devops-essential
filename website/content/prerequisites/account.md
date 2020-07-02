---
title: "Create an AWS account"
chapter: false
weight: 1
---

{{% notice warning %}}
Your account must have the ability to create new IAM roles and scope other IAM permissions.
{{% /notice %}}

1. If you don't already have an AWS account with Administrator access: [create
one now by clicking here](https://aws.amazon.com/getting-started/)

1. Once you have an AWS account, ensure you are following the remaining workshop steps
as an IAM user with administrator access to the AWS account:
[Create a new IAM user to use for the workshop](https://console.aws.amazon.com/iam/home?#/users$new)

1. Enter the user details:
![Create User](/images/iam-1-create-user.png)

1. Attach the AdministratorAccess IAM Policy:
![Attach Policy](/images/iam-2-attach-policy.png)

1. Click to create the new user:
![Confirm User](/images/iam-3-create-user.png)

1. Take note of the login URL and save:
![Login URL](/images/iam-4-save-url.png)


**Configure AWS CodeCommit:** The easiest way to set up AWS CodeCommit is to configure HTTPS Git credentials for AWS CodeCommit. On the user details page in IAM console, choose the **Security Credentials** tab, and in **HTTPS Git credentials for AWS CodeCommit**, choose **Generate**. 
![HTTPS Git Credential](/images/codecommit-iam-gc1.png)
        **💡 Note:** Make Note of the Git HTTP credentials handy. It will be used for cloning and pushing changes to Repo.
          Also, You can find detail instruction on how to configure HTTPS Git Credential [here](https://docs.aws.amazon.com/codecommit/latest/userguide/setting-up-gc.html)
* **IAM Permissions:** Finally, for the AWS account ensure you have sufficient privileges. 

You must have permissions for the following services:

* AWS Identity and Access Management
* Amazon Simple Storage Service
* AWS CodeCommit
* AWS CodeBuild
* AWS CloudFormation
* AWS CodeDeploy
* AWS CodePipeline
* AWS Cloud9
* Amazon EC2
* Amazon SNS
* Amazon CloudWatch Events

***

### **Important:**
The preferred region for this lab
- Stockholm (eu-north-1)

Stick to the same region throughout all labs. 
**Make sure you have not reached the VPC or Internet Gateway limits for that region. If you already have 5 VPCs/IGWs, delete at least one before you proceed or choose an alternate region.** 