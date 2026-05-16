# Udacity Submission Notes

## Website URLs

- S3 website endpoint:
- CloudFront endpoint:

## Required Screenshots

Place screenshots in `submission/screenshots/` before creating the final archive.

1. S3 bucket showing uploaded website files.
2. S3 static website hosting configuration showing the endpoint.
3. S3 bucket policy or permissions showing public read access.
4. CloudFront distribution showing the origin and deployed/enabled status.
5. Browser loading the site through the CloudFront endpoint.

## Deployment Commands

```bash
export AWS_REGION=us-east-1
export BUCKET_NAME=<globally-unique-bucket-name>
./scripts/deploy.sh "$BUCKET_NAME"
```
