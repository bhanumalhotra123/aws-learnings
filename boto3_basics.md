Getting Started with AWS Boto3 in Python

Boto3 helps you interact with AWS services programmatically, making your life a whole lot easier. Let's get started with some basics!

🌟What is Boto3?

Boto3 is the AWS SDK for Python, allowing you to interact with AWS services and resources using Python code. Whether you're managing EC2 instances, working with S3 buckets, or configuring IAM users, Boto3 provides an easy-to-use and object-oriented API.

🧑‍💻Logging into the AWS Management Console

You can log into the AWS Management Console using your IAM (Identity and Access Management) username and password.

But, if you want to interact with AWS programmatically, Boto3 comes to the rescue!

💡 Installing Boto3 and AWS CLI
To start, make sure you have Boto3 and AWS CLI installed:

pip3 install boto3
pip3 install awscli

🔧 Configuring AWS CLI
Configure AWS CLI using your access key and secret access key. You can find these credentials in the IAM User settings on the AWS Management Console.

aws configure

Enter your access key.
Enter your secret access key.
Choose a default region.
Choose a default output format.

Creating Your First Boto3 Session
In Python, you can create a Boto3 session like this:

import boto3
session = boto3.session.Session()

🎨 Custom Sessions
Sometimes, different developers need different access permissions. To achieve this, create custom profiles using the AWS CLI and associate them with different policies. For instance:

aws configure --profile ec2profile
aws configure --profile s3profile

Then, you can create a custom session in Python using:

session_custom = boto3.session.Session(profile_name="s3profile")

This session will have the permissions associated with the "s3profile" profile.

Client vs. Resource(explained with examples in attachments)

Boto3 provides two APIs for interacting with AWS services:

Client: Original API abstraction, offering low-level AWS service access. All AWS service operations are supported by clients.

Resource: A newer API abstraction offering high-level, object-oriented access. However, not all AWS services are covered.

![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/240c2bff-6729-40b6-80db-208ca517663d)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/ef86428f-49d1-48e4-a14a-b562b1ca2c53)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/fd7e4d3e-9c92-4244-8f33-153b8426dae1)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/699e3aa0-f23b-4d90-9926-98be4cd29446)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/7ac17de1-9ea5-446c-a6de-805d2cb87e93)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/8e9e1172-d67f-4431-96fa-f69243ecc9cd)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/61fc9a40-34ef-4c33-b840-0945f8891dc4)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/410b01a1-35b7-46c9-8fee-848b3d609863)
