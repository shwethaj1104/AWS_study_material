VPC: virtual private cloud

![image](https://user-images.githubusercontent.com/107784718/213640097-09f38293-8678-423e-a207-2666028c6ba3.png)

Search for VPC service- info about VPC's, subnets, route tables etc
![image](https://user-images.githubusercontent.com/107784718/213640310-e652d90a-383e-4392-bd74-4ea40cb19eae.png)

we can go to subnets to view- private and public subnets
private/public IP iwll have CIDR range example:172.31.48.0/20- so is any of 0-20 ip is available we can assign it to our application/instance while creating them
each availability zone will have VPC which in turn will hav erange of CIDR(Range of IP's) where we can craete our instance
___________________________
![image](https://user-images.githubusercontent.com/107784718/213641666-5c69eccb-e373-49c9-9aaa-90330b18e912.png)

![image](https://user-images.githubusercontent.com/107784718/213641710-31853452-5f9e-4487-9cef-7586958b5c30.png)

![image](https://user-images.githubusercontent.com/107784718/213642099-8d3ea3e2-3d4d-4f21-9a21-9f49288b111c.png)

# VPC Endpoints

• Endpoints allow you to connect to AWSServices using a private network instead of the public www network
• This gives you enhanced security and lower latency to access AWS services
___
# Site-to-Site VPN
• On-premises: must use a Customer Gateway (CGW)
• AWS: must use a Virtual Private Gateway (VGW)
![image](https://user-images.githubusercontent.com/107784718/213642696-f5736c42-cfff-44bb-a0fd-9b59945c5148.png)
__
