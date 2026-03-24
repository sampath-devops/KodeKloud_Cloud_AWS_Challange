### This project will help to host the static website in s3 bucket 
Hosting a static website on Amazon S3 is a highly scalable, cost-effective, and low-maintenance solution for sites composed of HTML, CSS, and JavaScript files. The process involves configuring an S3 bucket for public access and enabling the static website hosting feature

## Key Advantages
    Cost-Effective: You only pay for the storage used, data transfer, and requests.
    Scalability & Performance: S3 is designed to automatically scale to handle high traffic volumes and offers high durability and availability.
    Low Maintenance: There are no web servers to manage or update, reducing operational overhead.

## Step-by-Step Guide
 # Create an S3 Bucket
    1. Navigate to the AWS Management Console and create a new S3 bucket.
    2. Choose a globally unique name for your bucket. If using a custom domain (e.g., example.com), the    bucket name must exactly match your domain name.
    3. Select an AWS Region.
    4. In the Block Public Access settings, you will need to disable Block all public access to allow  public web access, and acknowledge the warning.
 # Upload Website Files
    1. Open your newly created bucket and upload all your static website files (HTML, CSS, JS, images, etc.).
    2. You can use the console's upload feature or automate deployments using the AWS CLI.
 # Configure Bucket Policy for Public Access
        1. Go to the Permissions tab of your bucket and edit the Bucket policy.
        2. Add a policy that grants public s3:GetObject permission for all objects in your bucket, replacing YOUR_BUCKET_NAME with your actual bucket name:
                json
                {
                    "Version": "2012-10-17",
                    "Statement": [
                        {
                            "Sid": "PublicReadGetObject",
                            "Effect": "Allow",
                            "Principal": "*",
                            "Action": "s3:GetObject",
                            "Resource": "arn:aws:s3:::YOUR_BUCKET_NAME/*"
                        }
                    ]
                }

 # Enable Static Website Hosting
        1. Go to the Properties tab and find the Static website hosting section, then click Edit.
        2. Select Enable and choose Host a static website.
        3. Specify your Index document (e.g., index.html) and optionally an Error document (e.g., error.html).
        4. Save changes.
        
### Access Your Website After saving, the Static website hosting section will display a Bucket website endpoint URL (e.g., http://your-bucket-name.s3-website-region.amazonaws.com).
You can access your live static website using this endpoint. 

Objects or files which are uploaded in S3 bucket

![Files in S3 bucket](image.png)

Below screenshot shows the static website which hosted in S3 bucket by following above steps

![Index](image.png)
![Project Page](image.png)


## Enhance Your Website by using below advanced concepts : We did not use in this simple project
       1. Use a Custom Domain: Map your domain name to the S3 endpoint using Amazon Route 53 for a user-friendly URL.
       2. Enable HTTPS/SSL: S3 website endpoints only support HTTP. To use HTTPS for security, you should configure an Amazon CloudFront distribution in front of your S3 bucket. CloudFront also acts as a Content Delivery Network (CDN) to improve performance and security.