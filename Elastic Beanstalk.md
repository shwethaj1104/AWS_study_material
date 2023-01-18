# Developer problems on AWS

• Managing infrastructure
• Deploying Code
• Configuring all the databases, load balancers, etc
• Scaling concerns

# AWS Elastic Beanstalk Overview 

• Elastic Beanstalk is a developer centric view of deploying an application on AWS
• It uses all the component’s we’ve seen before: EC2, ASG, ELB, RDS, etc...
• We still have full control over the configuration
• Beanstalk is free but you pay for the underlying instances

Elastic Beanstalk Managed service - Instance configuration / OS is handled by Beanstalk, Deployment strategy is configurable but performed by Elastic Beanstalk, capacity, load balancing, auto scaling, app health monitoring and responsiveness

Developer responsibility - just the applicatio code!
___
select Elastic beanstaclk service - craete application
![image](https://user-images.githubusercontent.com/107784718/213115154-12a25bae-659b-49d5-8d68-ab2b00062bf9.png)

![image](https://user-images.githubusercontent.com/107784718/213115419-3f6d4a42-65ed-4f39-836a-1ed66a0e534c.png)

application name- platform- platform branch- platform version-sample application

![image](https://user-images.githubusercontent.com/107784718/213115613-12402aff-b3b1-4551-9ad8-7551dde2d1a3.png)

open cloudformation service to check whta is happening
![image](https://user-images.githubusercontent.com/107784718/213115921-d3b2ca47-90f2-414a-89ba-3700e114cce6.png)
we can see our demp app is creating:
![image](https://user-images.githubusercontent.com/107784718/213116151-7f6c18fc-2803-4b76-a0d7-9a41602666c5.png)

if we view on design we can see template diagram: it has elastic load balancer,coud formation, security group,auto scaling, ec2 instance,cloud watch.
![image](https://user-images.githubusercontent.com/107784718/213116445-7d03ba63-a78d-4a8f-8228-1fa94bfab891.png)
