# Coveo DevOps Challenge
### The Challenge
Your challenge, should you choose to accept it, is to develop an AWS S3 storage analysis tool. To test your tool, you will have to create a free [Amazon](http://aws.amazon.com/en/free/) account (if you don't already have one).
### Specifications
The tool is a shell command (could be either Windows, Mac or Linux) that returns informations over all [S3](https://aws.amazon.com/documentation/s3/) buckets in an Amazon account.
##### The tool must returns the following informations:
- Bucket name
- Creation date (of the bucket)
- Number of files
- Total size of files
- Last modified date (most recent file of a bucket)

##### The following options shall be supported:
- Ability to get the size results in bytes, KB, MB, ...
- Organize the information by [storage type](https://docs.aws.amazon.com/AmazonS3/latest/dev/storage-class-intro.html) (Standard, IA, RR)
- Filter the results to a list of buckets (bonus point for regex support)
- Ability to group information by [regions](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)

##### Some additional features that could be useful (optional)
It would be nice to support prefix in the bucket filter (e.g.: s3://mybucket/Folder/SubFolder/log*). It may also be useful to organize the results according to the [encryption type](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingEncryption.html), get additional buckets informations (life cycle, cross-region replication, etc.) or take account of the [previous file versions](https://docs.aws.amazon.com/AmazonS3/latest/UG/enable-bucket-versioning.html) in the count + size calculation.

Some statistics to check the percentage of space occupied by a bucket or any other good ideas you could have are more than welcomes.
### Rules
- Your are free to use the programming language and the [SDK](https://aws.amazon.com/tools/) of your choice.
- We will test your work over our environment (which contains millions of files). The overall performance of your tool will be evaluated.
- Your code must be made available as a git fork of our challenge or any other public version control software.  
