# aws-cloud-security-lab
AWS S3 bucket configuration, IAM policies, and static website deployment with security best practices

## Objective
Configure secure AWS S3 buckets with least-privilege IAM policies, deploy a static website via CloudFront, and document security controls.

## Tools Used
- AWS CLI
- S3 Buckets
- IAM Policies
- CloudFront
- AWS Management Console

## Architecture
[User] → [CloudFront CDN] → [S3 Bucket (Private)] → [Origin Access Control]

text

## Steps Completed
1. Created S3 bucket with public access blocked
2. Configured IAM policies following least-privilege principle
3. Uploaded static website files
4. Deployed CloudFront distribution with OAC
5. Verified website access only through CloudFront

## Security Controls Implemented
- Bucket policy restricting access to CloudFront only
- IAM user with read-only permissions
- Server-side encryption enabled
- Access logs enabled for audit

## Lessons Learned
- Never make S3 buckets public – use CloudFront as CDN with OAC
- IAM policies should be as restrictive as possible
- Always enable logging for compliance and incident investigation

## Files
- `/policies/s3-bucket-policy.json`
- `/policies/iam-user-policy.json`
- `/docs/deployment-guide.md`

## Status
✅ Completed
