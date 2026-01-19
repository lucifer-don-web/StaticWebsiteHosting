Static Website Hosting on AWS S3
A simple, highly available static website hosted using Amazon S3. This project demonstrates how to configure an S3 bucket to serve web content (HTML and CSS) to the public internet without managing a traditional server.

Features
Serverless: No EC2 instances or servers to manage.

Highly Available: Leverages AWS S3 infrastructure for 99.99% availability.

Public Access: Configured with custom bucket policies for global reach.

Tech Stack
Storage: Amazon S3

Frontend: HTML5, CSS3

Security: AWS Identity and Access Management (IAM) Bucket Policies

Project Configuration
1. Bucket Setup
Bucket Name: static-web-op

Region: us-east-1 (N. Virginia)

Public Access: All "Block Public Access" settings were turned OFF to allow the website to be reachable.

2. File Structure
The following files were uploaded to the root directory of the bucket:

index.html: The main landing page.

style.css: Contains the styling for the page layout.

3. Website Hosting Configuration
Static Website Hosting: Enabled

Index Document: index.html

Endpoint: http://static-web-op.s3-website-us-east-1.amazonaws.com

4. Permissions (Bucket Policy)
To allow public read access, the following JSON policy was applied to the bucket:

JSON
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::static-web-op/*"
        }
    ]
}
Preview
The final output is a clean, centered webpage hosted directly from the S3 endpoint.