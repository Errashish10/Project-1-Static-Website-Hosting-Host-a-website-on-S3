# Project-1-Static-Website-Hosting-Host-a-website-on-S3

Step 1: Create and Configure S3 Bucket
Create S3 bucket:

Go to S3 > Create bucket

Name: yourdomain.com

Region: e.g., us-east-1

Uncheck “Block all public access”

Enable static website hosting:

In bucket > Properties > Enable Static Website Hosting

Index document: index.html

(Optional) Error document: error.html

Upload website files:

Go to Objects > Upload

Upload all your static files (HTML/CSS/JS/images)

Set permissions:

Add a Bucket Policy to allow public read access:

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::example.com/*"
    }
  ]
}

<img width="1335" height="454" alt="image" src="https://github.com/user-attachments/assets/15c9025a-ce77-4b16-8351-83931bfb756e" />
<img width="1353" height="529" alt="image" src="https://github.com/user-attachments/assets/c997ba64-6dbc-4682-b2d1-1450cdcf367d" />
<img width="1342" height="567" alt="image" src="https://github.com/user-attachments/assets/aee06aef-8e19-4ba4-80d2-61906d41c0ae" />





