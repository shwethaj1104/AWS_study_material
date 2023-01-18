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
![image](https://user-images.githubusercontent.com/107784718/213116946-730dd19e-a17d-4774-9632-502adef4de4b.png)

if we view on designer we can see template diagram: it has elastic load balancer,coud formation, security group,auto scaling, ec2 instance,cloud watch.
![image](https://user-images.githubusercontent.com/107784718/213116445-7d03ba63-a78d-4a8f-8228-1fa94bfab891.png)

if w ecome back to elastic beanstalk we can see what and all are created 
![image](https://user-images.githubusercontent.com/107784718/213117111-797a97fd-4785-4f66-ace8-52b1d45874d5.png)

once it is successfully created, click on link given to see the running application

you can even go to EC2 instances and check for the instance craeted by beanstalk(go to tags to find cloudformation tag)
![image](https://user-images.githubusercontent.com/107784718/213121014-547d4b61-c568-4752-bc4a-688ac932990b.png)

we can just upload and deploy new file to update application

difference between cloudformationa dn elastic beanstalk
coudformation is infrastructure focused where as EBS is application focused- we write what services to include via code for cloudformation where as we deploy application code in EBS

