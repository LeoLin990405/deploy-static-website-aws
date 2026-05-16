# Udacity Submission Notes

## Website URLs

- S3 website endpoint: http://leolin-udacity-static-website-835207447818-20260516.s3-website-us-west-2.amazonaws.com
- CloudFront endpoint: https://d1i5pbmzhtp53l.cloudfront.net

## Required Screenshots

Place screenshots in `submission/screenshots/` before creating the final archive.

1. S3 bucket showing uploaded website files.
2. S3 static website hosting configuration showing the endpoint.
3. S3 bucket policy or permissions showing public read access.
4. CloudFront distribution showing the origin and deployed/enabled status.
5. Browser loading the site through the CloudFront endpoint.

## Submitted Evidence

- `submission/screenshots/cloudfront-website.png` shows the deployed website loaded through CloudFront.
- `submission/evidence/s3-uploaded-files.json` shows objects uploaded to the S3 bucket.
- `submission/evidence/s3-website-configuration.json` shows static website hosting configuration.
- `submission/evidence/s3-bucket-policy.json` shows the public read bucket policy.
- `submission/evidence/cloudformation-resources.json` shows the S3 bucket, bucket policy, and CloudFront distribution resources.
- `submission/evidence/cloudformation-outputs.json` records the final S3 and CloudFront endpoints.
- `submission/evidence/cloudfront-distribution.json` shows the CloudFront distribution domain, origin, and deployed status.

## Deployment Commands

```bash
export AWS_REGION=us-east-1
export BUCKET_NAME=<globally-unique-bucket-name>
./scripts/deploy.sh "$BUCKET_NAME"
```
