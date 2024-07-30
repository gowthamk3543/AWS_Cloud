### Step 1 
– Created and Login to AWS console (As per recommended we need to login as IAM-user)


### Step 2 
- Search for EC2 select launch instance
Give Name - select OS image (AMI) - instance type - Create key pair - Launch instances

### Step 3
- After Creation we need to add security groups  
Select security - security groups - edit inbounds rules - add rules HTTP & anywhere IPv4

### Step 4
- Select instance - Now copy Public IPv4 address – open mobaxterm - select sessions & ssh then enter IP address - specify username - then provide additional SSH settings - give USE Private KEY (key pair) - then click OK

### EC2 instance EC2_Creation Connected in Mobaxterm
