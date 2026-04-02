markdown
# AWS Cloud Security Lab – Deployment Guide

## Prerequisites
- AWS account (free tier)
- Basic familiarity with AWS Console

## Steps Completed
1. Created S3 bucket with public access blocked
2. Uploaded index.html to bucket
3. Created CloudFront distribution with OAC
4. Updated S3 bucket policy to allow CloudFront access
5. Verified CloudFront URL works
6. Verified direct S3 URL returns Access Denied
7. Created IAM least-privilege policy
8. Created IAM user with policy attached

## Security Controls Implemented
- S3 bucket: Private, all public access blocked
- CloudFront: OAC ensures only CloudFront can access S3
- IAM policy: Least-privilege permissions
- HTTPS: Enforced for all traffic

## Author
Bemvindo Ntambu – IT Support & Cybersecurity Professional
