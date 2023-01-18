# CodeDeploy
deploy our application automatically
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
![image](https://user-images.githubusercontent.com/107784718/213130750-5cfa86a0-73d6-47f3-bfa6-463c34f72371.png)
____________
# CodeStar
• Unified UI to easily manage software development activities in one place
• “Quick way” to get started to correctly set-up CodeCommit, CodePipeline, CodeBuild, CodeDeploy, Elastic Beanstalk, EC2, etc...
• Can edit the code ”in-the-cloud” using AWS Cloud9
_________________
# Cloud9
AWS Cloud9 is a cloud IDE (Integrated Development Environment) for writing, running and debugging code
