### Step 1 – Login to AWS console (For best practice we need to login as IAM-user)
![p1](https://github.com/user-attachments/assets/629fe33a-875b-4512-b531-b94f44963975)

### Step 2 - Search for EC2 select launch instance
![p3](https://github.com/user-attachments/assets/3b2ce004-ee40-4fd7-8b25-0f4cd2347aca)
Give Name - select OS image (AMI) - instance type - Create key pair - Launch instances
![p4](https://github.com/user-attachments/assets/5639ca69-9b0b-459a-9d9f-ec4ec01bcdef)
![p5](https://github.com/user-attachments/assets/13ca7371-cd02-40b4-9fc1-76d2aa99cb4b)
![p6](https://github.com/user-attachments/assets/aab9bd2d-5f7e-40f3-90da-e9f21b30a350)

### Step 3- After Creation we need to add security groups  
### Select security - security groups - edit inbounds rules - add rules HTTP & anywhere IPv4
![p7](https://github.com/user-attachments/assets/273fa915-9ce7-4d27-b9dc-966f1ce0fa12)
![p8](https://github.com/user-attachments/assets/68618044-d7d0-4801-9a89-1a9a22ca1026)

### Step 4- Select instance - Now copy Public IPv4 address – open mobaxterm - select sessions & ssh then enter IP address - specify username - then provide additional SSH settings - give USE Private KEY (key pair) - then click OK
![p9](https://github.com/user-attachments/assets/3cd39a34-8ab3-425f-a4a9-5db18ab63349)
![p10](https://github.com/user-attachments/assets/cd63ff30-9174-4d37-9ea2-b7a4b9c5f571)
![p11](https://github.com/user-attachments/assets/e4b4fb9c-e8d1-46a8-a7ab-54574f06d474)

### EC2 instance EC2_Creation Connected in Mobaxterm
