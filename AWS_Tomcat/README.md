![image](https://github.com/user-attachments/assets/97cf03d7-40f4-49a6-8633-083c45b81030)### Install Tomcat web application server in AWS EC2 Ubuntu Instance and access Tomcat using a web browser
- To install Tomcat, we need to have EC2 instances follow below steps
- Login to AWS console (As a best practice we need to login as IAM-user)
- Search for EC2 - select launch instance
- Give Name - select OS image (AMI) - instance type - Create key pair - Launch instances
- In order to make connection secure we need to add some rules in security groups
- Select security - security groups - edit inbounds rules - edit present SSH custom (My IP) - add rule type (SSH) custom (give regional IP) - save rules
- Now Click on connect and again click on connect, now your connected to EC2 instance

- For tomcat Java is mandatory
- We need to install java before we install tomcat9
- By using: apt install openjdk-17-jdk -y

- Get tar link from website Apache tomcat9 
- By using: Wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.93/bin/apache-tomcat-9.0.93.tar.gz

- After getting file we need to Extract it
- By using: tar –xvzf apache-tomact-9.0.93.tar.gz

- Now remove apache-tomcat-9.0.93.tar.gz – Run rm apache-tomcat-9.0.93.tar.gz

- Select security - security groups - edit inbounds rules - add rules custom TCP, 8080 & anywhere IPv4 - save rule

- Change directory - Run cd apache-tomcat-9.0.93
- Run ls command and go to bin
- By using: cd bin
- After coming to bin directory
- Here we can start tomcat9
- By using: sh startup.sh

- Now find Public IP address and open new page in chrome
- Here you need to paste Public IP address along with 8080
- Ipaddress:8080

