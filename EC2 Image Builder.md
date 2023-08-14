# EC2 Image Builder

    • Used to automate the creation of Virtual Machines or container images

    • Automate the creation(EC2 instance and/or IAM etc), maintain, validate and test EC2 AMIs

    • Can be run on a schedule (weekly, whenever packages are updated, etc...)
_______________________________________________________________________________________________________________________
# EC2 image builder service

Create image pipeline
![image](https://user-images.githubusercontent.com/107784718/212533280-adbea58f-4369-45e9-aad8-12d96b907343.png)

Pipeline name -> Give time -> Choose recipe
An image recipe is a document that defines the components to be applied to the base images to create the desired configuration for the output image. After a recipe has been created, it cannot be modified. A new version must be created in order to change components.

![image](https://user-images.githubusercontent.com/107784718/212533413-93dbb0b1-39cf-4929-a83a-83b6297a9f9b.png)

AMI -> Name -> Version -> Amazon linux -> Image name (amazon linux 2 x86) -> Add components
![image](https://user-images.githubusercontent.com/107784718/212533499-4360ec2d-afd5-45bf-bc83-e4760b79f0fa.png)
(for java -> Amazon-corretto-11-headless
aws-cli-version-2-linuxamazon-corretto-11-headless)

Next -> 
Infrastucture configurations -> Create a new infra configs -> Name -> Select IAM role if exist else create new IAM role 
_________________________
Create new IAM role -> Name
Add Policies- EC2InstanceProfileForImageBuilder,EC2InstanceProfileForImageBuilderECRContainerBuilds,AmazonSSMManageInstanceCore
____________________________
Distributions settings- either default/ (new one- and assign to various regions)- create pipeline
_____________________________
once it is craeted- tested- distributes
launch an instance and connect via available AMI- select your AMI- and connect to the instance- you now have your instance up and running
