# Code Deploy

Deploy our application automatically
• Works with EC2 Instances
• Works with On-Premises Servers
• Hybrid service
________________
# CodeCommit 
• Before pushing the application code to servers, it needs to be stored somewhere
• Developers usually store code in Git
• A famous public offering is GitHub, AWS’s competing product is CodeCommit
______________
# CodeBuild
Compiles source code, run tests, and produces packages that are ready to be deployed (by CodeDeploy for example)
_____________
# CodePipeline
Orchestrate the different steps to have the code automatically pushed to production
• Code => Build => Test => Provision => Deploy
• Basis for CICD (Continuous Integration & Continuous Delivery)
______________
# CodeArtifact
• Software packages depend on each other to be built (also called code dependencies), and new ones are created
• Storing and retrieving these dependencies is called artifact management
• Traditionally you need to setup your own artifact management system
• CodeArtifact is a secure, scalable, and cost-effective artifact management for software development
• Works with common dependency management tools such as Maven, Gradle, npm, yarn, twine, pip, and NuGet
• Developers and CodeBuild can retrive it from CodeArtifact

We can setup Individually too, but we have CodeStar where we can setup all of them at once,
![image](https://user-images.githubusercontent.com/107784718/213138269-844923c2-f110-4e0b-b78c-13a8dcb201d2.png)

____________
# CodeStar
• Unified UI to easily manage software development activities in one place
• “Quick way” to get started to correctly set-up CodeCommit, CodePipeline, CodeBuild, CodeDeploy, Elastic Beanstalk, EC2, etc...
• Can edit the code ”in-the-cloud” using AWS Cloud9

open CodeStar service- create project-select the application type(eample python flask-AWS Elastic Beanstalk)- Next
![image](https://user-images.githubusercontent.com/107784718/213131078-a3f70a05-bc12-4dc4-8910-85c2353a0a0d.png)

![image](https://user-images.githubusercontent.com/107784718/213131310-e163fe52-1410-4b45-9750-7679569aed18.png)

project name-project repository:codeCommit-EC2 configuration:::instance type:t2 micro-select subnet-select key pair--next
project will be created- with AWS IAM, Elastic Beanstalk, CodePipeline, CodeCommit,CodeBuild,CloudFormation and Amazon S3 storage.
_________________
# Cloud9
AWS Cloud9 is a cloud IDE (Integrated Development Environment) for writing, running and debugging code

after creating codestar project- go to craete Could9- environment name-create environment

once cloud9 env is craeted-
click on Open IDE-we will get cloud9 which will be running on web browser we can edit code on browser
to commit code -> Edit the code- Click on left corner "git" in cloud9 IDE-on changed file click + -> enter user message- ctrl enter(file has been commited now)
to push code to git-> on cloud9 terminal- go to root directory of project- git push

Once new changes are pushed to codcommit- changes will be automatically deployed! since the pipeline in codeStar will be automatically triggered whne there is changes!
