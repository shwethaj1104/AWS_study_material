# What is Docker?

• Docker is a software development platform to deploy apps.

• Apps are packaged in containers that can be run on any OS.

• Apps run the same, regardless of where they’re run ->

        • Any machine 
        • No compatibility issues 
        • Predictable behavior 
        • Less work 
        • Easier to maintain and deploy 
        • Works with any language, any OS, any technology 
        
• Scale containers up and down very quickly (seconds).

Ways to luanch docker on AWS ->
_____________________________________________________________________________________________________________________________________________________________________________
# ECS-Elastic Container Service

• Launch Docker containers on AWS.

• You must provision & maintain the infrastructure (the EC2 instances).
_____________________________________________________________________________________________________________________________________________________________________________
# Fargate 

• Launch Docker containers on AWS

• You do not provision the infrastructure (no EC2 instances to manage) – simpler!

• Serverless offering (Serverless does not mean there are no servers... it means you just don’t manage / provision / see them)
• AWS just runs containers for you based on the CPU / RAM you need
___________
# ECR - Elastic Container Registry 

• Private Docker Registry on AWS
• This is where you store your Docker images so they can be run by ECS or Fargate
