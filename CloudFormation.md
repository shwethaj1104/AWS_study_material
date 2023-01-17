• CloudFormation is a declarative way of outlining your AWS
Infrastructure, for any resources (most of them are supported).
• For example, within a CloudFormation template, you say:
• I want a security group
• I want two EC2 instances using this security group
• I want an S3 bucket
• I want a load balancer (ELB) in front of these machines

• Then CloudFormation creates those for you, in the right order, with the
exact configuration that you specify.

No resources are manually created, which is excellent for control.
