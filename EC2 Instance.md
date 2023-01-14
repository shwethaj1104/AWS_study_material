EC2 = Elastic Compute Cloud = Infrastructure as a Service
It mainly consists in the capability of :
• Renting virtual machines (EC2)
• Storing data on virtual drives (EBS)
• Distributing load across machines (ELB)
• Scaling the services using an auto-scaling group (ASG)

go to EC2 service:
![image](https://user-images.githubusercontent.com/107784718/212465702-deb83975-79df-453f-93b4-1b7ea2445fb5.png)

Click on - instances- Launch instances
![image](https://user-images.githubusercontent.com/107784718/212465736-622c4332-5a3c-4eb2-a40a-1b624886e5d6.png)

Give name - select Amazon Linux as application- use Amazon Linux 2 AMI (HVM)-64-bit(x86)-free to use
![image](https://user-images.githubusercontent.com/107784718/212465808-b43fa300-d150-4c36-9364-641d3e0fabd8.png)

Instance type- t2-micro--free to use

key pair- click on-- create new key pair-name-
if MAC/WINDOWS>10 --Use .pem
If Windows<10 --use .ppk
![image](https://user-images.githubusercontent.com/107784718/212465996-68b104cf-7c19-4018-91f5-16d95d40b1b4.png)
Once key pair is created it will be automatically selected

Network security:
![image](https://user-images.githubusercontent.com/107784718/212466079-95a514fb-dc1e-4033-a7c2-9b961eb5ba14.png)

Storage(volumes):

![image](https://user-images.githubusercontent.com/107784718/212466103-ae82f868-a848-4380-ba42-6b0451046b32.png)

On termination of the instance the volume will be deleted--control is over here we can change that too

![image](https://user-images.githubusercontent.com/107784718/212466121-120ee024-b618-4205-80b0-623291e650f6.png)

Advanced details:

when ever you want to execute a script when the isntance is first started-only once in whole life cycle of install give the commands in--User data
![image](https://user-images.githubusercontent.com/107784718/212466235-d9098838-3ad2-4fd5-a75f-5c1aaf934578.png)

Launch Instance

![image](https://user-images.githubusercontent.com/107784718/212466284-dc1a57b4-087e-4b8a-9160-a0854789301b.png)

in the list f instances now we can see the newly craeted instance
![image](https://user-images.githubusercontent.com/107784718/212466302-74e17831-f504-42b2-a459-5fe08eac9caf.png)

