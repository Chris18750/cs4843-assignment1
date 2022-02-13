# cs4843-assignment 1
This Github respository contains the source code for a website that uses the Amazon Web Services S3 web service to store these files and the Amazon CloudFront to deliver these files. This cloud infrastructure is used in order to host this website and is secured using IAM Policies.

## Table of contents
* [Website Structure](#website-structure)
* [S3](#s3)
* [Cloud Front](#cloud-front)
* [Policies](#policies)
* [Website Access](#access)

## Website Structure
The website contains 5 pages created through HTML and contains multiple pictures and one video.

## S3
The project uses Amazon Web Services S3 web service to store the necessary files to display the web content. AWS S3 is a cloud object storage service that allows you to store and retrieve files from anywhere. The project uses this form of storage, becuase the website is a static website and AWS S3 allows simple storage and retrieval of these files. All the files listed in this github repository are hosted in a S3 bucket and can be retrieved to display the website.

## Cloud Front
This project uses the AWS CloudFront in order to speed up content delivery. The AWS CloudFront is a content delivery network that caches content and stores the cached content in servers around the world. This allows for low latency and higher security for projects that uses the AWS CloudFront for delivering content.
The projects AWS S3 buckect is linked to the the AWS CloudFront alowing all the files needed to host the website to be deliverd with low latencey arround the world.

## Policies
Policies are used in AWS in order to set permissions for users. This project uses an AWS policy that only allows the AWS CloudFront to get any object within the AWS S3 bucket used for storing the website's files. Any user can get theses files only if they have the correct URL provided by the AWS CloudFront that is linked to the project's AWS S3 bucket.

## Website Access
The website can be accessed using the following URL
https://d1kmp53kdtnsd8.cloudfront.net/
