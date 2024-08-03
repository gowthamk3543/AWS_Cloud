# Launch EC2 and try to transfer file to S3

### we need to create IAM user with roles as EC2 full access and S3 full access after creation we'll get to see Access key, generate it and download csv.file where our access key details will be there
For Creating IAM user please do check AWS_IAM file
### Launch EC2  instance and connect in mobaxterm
For detailed steps of EC2 creation check AWS_EC2 file
![image](https://github.com/user-attachments/assets/74712727-3ec2-4327-b8f9-f3851f37700f)
### Switch it to root user sudo -i
### update the terminal apt update - y
### Now we need to install unzip apt install upzip - y
![image](https://github.com/user-attachments/assets/2017e05f-10f1-426b-8b05-32e255f488c4)
![image](https://github.com/user-attachments/assets/2b52afcc-6f66-4da7-83c8-0344c15d52b1)
### Now we need to install aws cli go to Google search aws cli install in linux we will get link paste in terminal 
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"  
unzip awscliv2.zip  
sudo ./aws/install
### To verify aws - - version
### Now we need to configure AWS - aws configure 
### We need to provided access key, secret key, region and format of output like json file
### Now we have configured aws 
![image](https://github.com/user-attachments/assets/dd2639ef-d040-4b24-bbc7-f51f0a5115ec)
![image](https://github.com/user-attachments/assets/60b12581-bb81-4a4f-b310-0819f2f28154)
### Now we will created s3 bucket for that we use aws s3 mb s3://buck-name
### To verify aws s3 ls
### Now create new file echo "this is the file to add in S3 bucket" > samplefile.txt
### Now add this file to S3 bucket aws s3 cp samplefile.txt s3://bucket-name
### To verify aws s3 ls s3://bucket-name
![image](https://github.com/user-attachments/assets/de309d37-ad20-499d-8ee3-c460a54bfe80)
![image](https://github.com/user-attachments/assets/bb26f6a3-dfcf-4dca-85d2-37f5d5b74c70)
### This is how we add files to s3 from ec2
