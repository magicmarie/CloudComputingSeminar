# Homework 1: Exploring AWS Services

## Set up an AWS Free Tier Account:

* If you do not already have one, create an AWS Free Tier account to access AWS services.

* Turn on MFA for a root account

* Setup a billing Alert using CloudWatch to monitor your AWS expense

* Setup a budget alert for monthly expense

## Create an Amazon S3 Bucket and Upload a File

* Create a new S3 bucket in your AWS account. Ensure the bucket name is unique.

* Uncheck the "Block Public Access"

* Navigate to the `properties` tab in the S3 bucket console and enable `Static website hosting`.

* Upload the file `index.html` with the following content:

```

<html>

<body>

<h1> Hello AWS! </h1>

</body>

</html>

```

* Update the bucket policy with the policy below:

{

"Version": "2012-10-17",

"Statement": [

{

"Sid": "PublicReadGetObject",

"Effect": "Allow",

"Principal": "*",

"Action": "s3:GetObject",

"Resource": "arn:aws:s3:::your-bucket-name/*"

}

]

}

## Submit screenshots demonstrating:

* The billing alert

* The budget alert

* The S3 bucket with the uploaded file.

* The public URL of the index file.
