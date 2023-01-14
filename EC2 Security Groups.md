They control how traffic is allowed into or out of our EC2 Instances.
• Security groups are acting as a “firewall” on EC2 instances
they regulate: access to ports, control of inbound and outbound network

• If your application is not accessible (time out), then it’s a security group issue
• If your application gives a “connection refused“ error, then it’s an application
error or it’s not launched
• All inbound traffic is blocked by default
• All outbound traffic is authorised by default

In Network & security- Security groups- you will be able to see all the security groiups - we recently created launch-wizard-48- if we select it we will be able to see the inbound rules
(to check which wizard we are using- go to your isntance- scroll to right in your selected list of instance there you wil find a column of wizard)
![image](https://user-images.githubusercontent.com/107784718/212467101-153576c0-6042-458e-aa35-5173177a2186.png)

since in the wizard we have http rule- w ewere able to access the app from the browser

If you want to add or delete- seciroty inbounds- we can edit it too
![image](https://user-images.githubusercontent.com/107784718/212467212-d50643b1-8380-42d0-a134-f757501c1fc1.png)

Outbound traffic- by default to everywhere
![image](https://user-images.githubusercontent.com/107784718/212467313-0b590b0d-2d59-4cfc-8cb1-b47dc1a4960c.png)


We can attach as many securoty groups as we want to EC2 isntances.
