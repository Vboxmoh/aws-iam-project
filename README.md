# AWS IAM Project

## Project Overview
This project demonstrates the configuration of AWS Identity and Access Management (IAM) including users, groups, roles, and custom policies.

## Steps Completed

### 1. IAM User
Created an IAM user named john-doe with console access and attached the AmazonS3ReadOnlyAccess policy.

### 2. IAM Group
Created a group named Developers with AmazonS3ReadOnlyAccess and AmazonEC2ReadOnlyAccess policies. Added john-doe to the group.

### 3. IAM Role
Created a role named ec2-access-to-S3 with AmazonS3FullAccess policy and attached it to the EC2 instance. Tested permissions using the AWS CLI command aws s3 ls.

### 4. Custom Policy
Created a custom JSON policy named S3-ReadOnly-Custom-Policy granting read-only access to S3 using s3:GetObject and s3:ListBucket actions.

### 5. MFA
Enabled Multi-Factor Authentication for the IAM user john-doe using an authenticator app.

## Key Concepts Learned
- Identification vs Authentication vs Authorization
- Principle of Least Privilege
- IAM Users, Groups, Roles and Policies
- JSON policy documents
- MFA best practices

## Screenshots
All screenshots are available in the screenshots folder.

## Technologies Used
- AWS IAM
- AWS EC2
- AWS S3
- AWS CLI
