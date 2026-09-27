# AWS Cloud Security Lab

A hands-on cloud security project demonstrating a private Amazon S3 website delivered securely through Amazon CloudFront using Origin Access Control (OAC) and least-privilege IAM policies.

## Objective

Configure a secure AWS-hosted static website while preventing direct public access to the S3 bucket and documenting the implemented security controls.

## Tools Used

* AWS Management Console
* AWS CLI
* Amazon S3
* Amazon CloudFront
* AWS Identity and Access Management (IAM)

## Architecture

`User → CloudFront CDN → Origin Access Control → Private S3 Bucket`

## Steps Completed

1. Created an S3 bucket with public access blocked.
2. Configured IAM permissions following the least-privilege principle.
3. Uploaded the static website files.
4. Deployed a CloudFront distribution using OAC.
5. Updated the S3 bucket policy to permit CloudFront access.
6. Verified that the website is accessible through CloudFront.
7. Verified that direct access to the S3 bucket is denied.

## Security Controls Implemented

* Blocked all public access to the S3 bucket.
* Restricted bucket access to the CloudFront distribution.
* Applied least-privilege IAM permissions.
* Enabled server-side encryption.
* Enforced HTTPS through CloudFront.
* Enabled access logging for auditing and investigation.

## Lessons Learned

* Private S3 buckets can securely serve content through CloudFront and OAC.
* IAM permissions should be limited to only the required actions and resources.
* Public access prevention and logging improve security and auditability.
* Cloud resource identifiers should be replaced with placeholders before publishing configuration files.

## Project Files

* [S3 bucket policy](policies/s3-bucket-policy.json)
* [IAM least-privilege policy](policies/iam-user-policy.json)
* [Deployment guide](docs/deployment-guide.md)
* [Documentation index](docs/README.md)
* [Static website file](index.html)
* [Validation screenshots](screenshots/README.md)
## Status

✅ Completed
