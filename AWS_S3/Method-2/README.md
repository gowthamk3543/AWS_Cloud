# Launch EC2 and try to transfer file to S3

### we need to create IAM user with roles as EC2 full access and S3 full access after creation we'll get to see Access key, generate it and download csv.file where our access key details will be there

### Launch EC2  instance and connect in mobaxterm

### Switch it to root user sudo -i
### update the terminal apt update - y
### Now we need to install unzip apt install upzip - y

### Now we need to install aws cli go to Google search aws cli install in linux we will get link paste in terminal 
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"  
unzip awscliv2.zip  
sudo ./aws/install
### To verify aws - - version

### Now we need to configure AWS - aws configure 
### We need to provided access key, secret key, region and format of output like json file
### Now we have configured aws 

### Now we will created s3 bucket for that we use aws s3 mb s3://buck-name
### To verify aws s3 ls
### Now create new file echo "this is the file to add in S3 bucket" > samplefile.txt
### Now add this file to S3 bucket aws s3 cp samplefile.txt s3://bucket-name
### To verify aws s3 ls s3://bucket-name

### This is how we add files to s3 from ec2
