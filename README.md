# Static Website Hosting on AWS with S3 and CloudFront


<p align="center">
  <img src="https://github.com/user-attachments/assets/5b7dacf4-c846-4af0-9a24-57621c3203ff" width="514" height="268" alt="image" />
</p>


This project demonstrates how to host a static website on AWS using an S3 bucket as the origin and CloudFront as the CDN for fast and secure content delivery. It uses Origin Access Control (OAC) to restrict direct access to the S3 bucket and serve content only through CloudFront.

Steps to Deploy

1. Create an S3 Bucket
Create a new Amazon S3 bucket.
Configure the bucket to allow public access for hosting your website files.
Upload your website files (HTML, CSS, JavaScript, images, etc.) to the bucket.

2. Set Up CloudFront Distribution
Navigate to the AWS CloudFront console.
Create a new CloudFront distribution.
Select your S3 bucket as the origin.
Create and attach an Origin Access Control (OAC) to restrict direct S3 bucket access and serve content securely via CloudFront.

3. Configure CloudFront Settings
Set the Default Root Object (e.g., index.html) to specify the landing page.
Wait for the distribution to finish deploying.
[NOTE] - for the bucket policy they are given when the OAC is being produced so you can copy from there and use it

5. Launch Your Website
Access your website using the CloudFront distribution domain name.
Your website will now be served securely and quickly through CloudFront.
