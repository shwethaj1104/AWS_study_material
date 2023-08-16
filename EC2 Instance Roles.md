Go to your EC2 instance - select - Click on Connect- Connect

![image](https://user-images.githubusercontent.com/107784718/212468045-97f12fb0-0616-40fe-bbbc-e2f540207e53.png)

You will be navigated to new tab with console
try ping google.com
aws --version
aws iam list-users  --- do not configure your aws here- if you enter all key's - anyone from your account can connect to EC2 instances and retrieve the credentials here. 

Use IAM roles instead
Go to IAM- and check for required IAM role
Go to EC2 instance- click on it - there will be no IAM as of now
![image](https://user-images.githubusercontent.com/107784718/212468272-40a35599-dd93-45a8-8454-b936c221437f.png)

Go back to instances- Actions- Security- Modify IAM role
![image](https://user-images.githubusercontent.com/107784718/212468303-c3a65c08-056d-4a07-9693-897329bc00f3.png)

![image](https://user-images.githubusercontent.com/107784718/212468321-c9a20d0b-8650-447b-9fa4-c8bb3c954418.png)
select IAM role and - click update IAM Role
