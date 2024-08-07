### Install Tomcat web application server in AWS EC2 Ubuntu Instance and access Tomcat using a web browser
- To install Tomcat, we need to have EC2 instances follow below steps
- Login to AWS console (As a best practice we need to login as IAM-user)
- Search for EC2 - select launch instance
- Give Name - select OS image (AMI) - instance type - Create key pair - Launch instances
- In order to make connection secure we need to add some rules in security groups
- Select security - security groups - edit inbounds rules - edit present SSH custom (My IP) - add rule type (SSH) custom (give regional IP) - save rules
- Now Click on connect and again click on connect, now your connected to EC2 instance
![image](https://github.com/user-attachments/assets/a7b5713d-1002-4f8b-a052-dadede4140ce)
![image](https://github.com/user-attachments/assets/53e87b32-f31f-4aee-82a1-585f567ea5b9)
![image](https://github.com/user-attachments/assets/c25388b2-e1e8-45ca-8773-00a0361b655e)

Now we will see how to install Tomcat follow below steps
- In order to run commands, switch to root user
- sudo -i
- apt update -y 
![image](https://github.com/user-attachments/assets/71c9cda3-8184-4f63-aafd-7be82d09ffb5)

- For tomcat Java is mandatory
- We need to install java before we install tomcat9
- By using: apt install openjdk-17-jdk -y
![image](https://github.com/user-attachments/assets/34176d51-b73d-4176-9561-7d745e4ead0d)

- Get tar link from website Apache tomcat9 
- By using: Wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.93/bin/apache-tomcat-9.0.93.tar.gz
![image](https://github.com/user-attachments/assets/718ea79b-b9b5-4816-ab6b-f87c6f75525a)
![image](https://github.com/user-attachments/assets/e115285c-7929-4565-b265-b8784e9489db)

- After getting file we need to Extract it
- By using: tar –xvzf apache-tomact-9.0.93.tar.gz
![image](https://github.com/user-attachments/assets/7ed155eb-a04b-48e5-afd4-ce87a4672913)

- Now remove apache-tomcat-9.0.93.tar.gz – Run rm apache-tomcat-9.0.93.tar.gz
![image](https://github.com/user-attachments/assets/f1ffb031-d02e-40d2-b58d-0961c60743ec)

- Select security - security groups - edit inbounds rules - add rules custom TCP, 8080 & anywhere IPv4 - save rule
![image](https://github.com/user-attachments/assets/0edb686e-93a2-445f-9004-e6149806b1fd)

- Change directory - Run cd apache-tomcat-9.0.93
- Run ls command and go to bin
- By using: cd bin
- After coming to bin directory
- Here we can start tomcat9
- By using: sh startup.sh
![image](https://github.com/user-attachments/assets/38a6a4eb-e3d6-45e5-aeed-856520bbbac4)

- Now find Public IP address and open new page in chrome
- Here you need to paste Public IP address along with 8080
- Ipaddress:8080
![image](https://github.com/user-attachments/assets/a2a9c3d8-ce86-42e3-9cba-827db2563460)

