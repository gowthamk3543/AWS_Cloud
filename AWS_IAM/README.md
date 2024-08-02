# Login to AWS Console and Create IAM User, Role, and Group
### Step 1 - Login to AWS console
![p1](https://github.com/user-attachments/assets/aa19cc2e-053f-4a87-a8ab-578adde4dafe)
### Step 2 - Search & select IAM
![p2](https://github.com/user-attachments/assets/24c69905-9439-4729-868b-3344d09e6ff2)
# We will now see how to Create New User
### Step 3 - Now select Create user - provide username - select Provide user access to the AWS Management Console - choose console password (auto generated password) - choose Users must create a new password at next sign-in - click next
![p3](https://github.com/user-attachments/assets/9259dc9e-f5b8-4418-b7f7-d984db4b7cb1)
![p4](https://github.com/user-attachments/assets/daf2f605-ccb5-4a49-9a63-9df968921fae)
![p5](https://github.com/user-attachments/assets/ea303e50-8fc2-46ba-a8d3-6d8e39f8128f)
### Step 4 - Now we need to give permissions we have 3 options but for now we will select Attach policies directly - select permissions policies search policies and select - click next
![p6](https://github.com/user-attachments/assets/4c9d5f36-7b88-49ff-8213-0cfc6b18b096)
![p7](https://github.com/user-attachments/assets/5457b876-9d33-4c32-817d-550f0e1b9b4f)
### Step 5 - Now we need to review it and click CREATE USER 
![p8](https://github.com/user-attachments/assets/b57312f1-59af-43e8-a63e-122745aa4c7e)
### Step 6 - We will get link, username and password using this we can login to new user and this is the only time we get to see and download password so we need to share it via email or download .csv file
![p9](https://github.com/user-attachments/assets/c756ca03-30c3-40f7-8953-a503e54d972f)
![p10](https://github.com/user-attachments/assets/ca5a137e-9281-4bc1-837d-70d04e9652ef)
![p11](https://github.com/user-attachments/assets/91d681f2-437b-4ead-9d56-74805ab995b4)
![p12](https://github.com/user-attachments/assets/4b0697b4-b2e0-4406-8ef3-3b9987fefc91)
### We have created and logged IN: IAM_User_Creation 


# We will now see how to Create New Role
### Step 1 - Now select roles and click create role - select required Trusted entity type - select use case (adding services) - now click next - now add required permissions - click next - provide role name, tags review it and click create role
![Picture1](https://github.com/user-attachments/assets/a54ea8b7-a5c0-4d2d-8586-9a5fa557a275)
![Picture2](https://github.com/user-attachments/assets/30a1d104-d0c4-487d-bd82-b019100bc724)
![Picture3](https://github.com/user-attachments/assets/bd8db673-f080-4d3a-9c92-b452320c835e)
![Picture4](https://github.com/user-attachments/assets/9eb123ab-3fc4-4d06-befe-99f098016304)
![Picture5](https://github.com/user-attachments/assets/f513fa36-f5d7-4fa3-b222-09d74aac240a)
![Picture6](https://github.com/user-attachments/assets/a86d7138-df64-4e25-983b-e7f5ff7dccd7)
![Picture7](https://github.com/user-attachments/assets/1c9a8081-a082-4809-9b69-8bac759d79ae)
### We have created Role: IAM_Role_Creation


# We will now see how to Create New Group
### Step 1 - Now select group and click create group - provide group name - we can add available users to group - now Attach permissions policies as per need - then click create group

### We have created Group: IAM_Group_Creation
