Cloud formation -> yaml format

• CloudFormation is a declarative way of outlining your AWS Infrastructure, for any resources (most of them are supported).

• For example, within a CloudFormation template, you say:

            • I want a security group
  
            • I want two EC2 instances using this security group
            
            • I want an S3 bucket
            
            • I want a load balancer (ELB) in front of these machines

• Then CloudFormation creates those for you, in the right order, with the exact configuration that you specify.

No resources are manually created, which is excellent for control.
_________________________________________________________________________________________________________________________________________________________________________
Search for cloudformation service in AWS ->
![image](https://user-images.githubusercontent.com/107784718/212883333-2ed7d72c-f982-43c6-a4c4-ca2362c9324c.png)

Create stack ->
![image](https://user-images.githubusercontent.com/107784718/212883842-ead53f34-8a3f-4fb6-a480-9652bc7cba6c.png)

Upload a file (which should contain what stacks you need to add -> example -> EC2, SSH security groups etc) which containes code in yaml format to create EC2 instance for example -> Next
stack name- Next
Tags- Name- Next
Review the cost and other details- Create Stack

You can update the stack if you want after creating it- just click on Update button

What ever you update will be available in change set preview where you can verify your chnages before updating
