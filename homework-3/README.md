# MIU-Seminar-2025-03-Homework3
# Requirements
1. Setup EC2 Instances
* Launch 2 EC2 instances with Amazon Linux
- Install a web server using the command: sudo yum install nginx
- Start Nginx: sudo systemctl start nginx
- Change the file /user/share/nginx/html/index with the content below:
```
<html>
  <body>
    <h1> Hello from my server 1! </h1>
  </body>
</html>
```
- Allow HTTP traffic in the security group
* Access the website in the browser using url: http://Public-IP-of-Instance
2. Create an Application Load Balancer (ALB)
* Create a target group and add the above instances to it
* Create ALB with the above target group
* Test Load Balancing: Navigate the website using ALB DNS
* (Optional): Create an ASG which uses the above ALB
3. Create an S3 Bucket and CloudFront to host a static website.
* Create a S3 bucket
* Upload a simple HTML file
* Create a CloudFront Distribution linked to the S3 bucket
* Access the website using the CloudFront DNS
## Submit screenshots demonstrating:
* EC2 instances
* Websites from these EC2
* ALB
* Website from ALB DNS
* Target Group
* S3 Buckets
* CloudFront
* Website from CloudFront DNS
