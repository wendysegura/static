## Jenkins Pipelines on AWS Project Overview
Create and run an instance on AWS, configure Jenkins, and create a pipeline to deploy a static website on S3.

### Create a group on AWS with the following Policies:
* AmazonEC2FullAccess
* AmazonVPCFullAccess
* AmazonS3FullAccess

### Create a new User named jenkins on AWS
* create new key pair for the user
* launch an EC2 Ubuntu server,  install Jenkins

### Ensure that Jenkins is running
* `sudo systemctl status jenkins`

### Set up Jenkins
* http://your_server_ip:8080
* install plugins required
  * Blue Ocean, etc.

### Final Steps
* Create a pipepine
* Set up Github
* Connect AWS Credentials and Github to Jenkins
* Set up an S3 bucket with Public Policy attached to it
* Set up pipelines



