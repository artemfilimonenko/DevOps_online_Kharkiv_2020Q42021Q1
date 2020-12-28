# Module 2 
## Virtualization and Cloud Basic
### Task 2.2 AWS Core Services

<a href="http://filimonenkobucket.s3-website.eu-central-1.amazonaws.com/">My static website</a>
 
In the course of doing this labwork I had to sign up for a AWS account, get acquainted with AWS Free Tier limits and work with some AWS services.

The first step was to launch instance via Amazon Lightsail

<img src="./screenshots/1. lightsail AMI.jpg" width="90%"/>

Next step was to launch another Linux Virtual Machine without Amazon Lightsail. Made it via EC2 and connected to instance via SSH 

<img src="./screenshots/2.SSH connect to EC2 instance.jpg" width="90%"/>

Created a snapshot of my EC2 

<img src="./screenshots/3.made a snapshot.jpg" width="90%"/>

Then I created and attached EBS to my 1st instance

<img src="./screenshots/made EBS volume.jpg" width="90%"/>

<img src="./screenshots/mounted Disk_D & added some files.jpg" width="90%"/>

After that I launched my instance from backup, detached EBS of the previous instance and attached to it 

<img src="./screenshots/launch_backup.jpg" width="90%"/>

<img src="./screenshots/attaching_EBS volume to the 3rd instance.jpg" width="90%"/>

Created S3 bucket, also get acquainted with batch upload via CLI 

Added IAM permission

<img src="./screenshots/added iam permission.jpg" width="90%"/>

<img src="./screenshots/CLI_1.jpg" width="90%"/>

<img src="./screenshots/uploading via CLI.jpg" width="90%"/>

The last task was to create a static website on Amazon S3

<img src="./screenshots/WebSite_FINAL.jpg" width="90%"/>
http://filimonenkobucket.s3-website.eu-central-1.amazonaws.com





