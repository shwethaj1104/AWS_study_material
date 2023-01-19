# CloudWatch matrix

• CloudWatch provides metrics for every services in AWS
• Metric is a variable to monitor (CPUUtilization, NetworkIn...)

# Important Metrics

• EC2 instances: CPU Utilization, Status Checks, Network (not RAM)
• Default metrics every 5 minutes
• Option for Detailed Monitoring ($$$): metrics every 1 minute
• EBS volumes: Disk Read/Writes
• S3 buckets: BucketSizeBytes, NumberOfObjects, AllRequests
• Billing:Total Estimated Charge (only in us-east-1)
• Service Limits: how much you’ve been using a service API
• Custom metrics: push your own metrics

# Amazon CloudWatch Alarms
• Alarms are used to trigger notifications for any metric
• Alarms actions...
• Auto Scaling: increase or decrease EC2 instances “desired” count
• EC2 Actions: stop, terminate, reboot or recover an EC2 instance
• SNS notifications: send a notification into an SNS topic

# Amazon CloudWatch Logs
• CloudWatch Logs can collect log from:
• Elastic Beanstalk: collection of logs from application
• ECS: collection from containers
• AWS Lambda: collection from function logs 
• CloudTrail based on filter 
• CloudWatch log agents: on EC2 machines or on-premises servers
• Route 53- log DNS queries
• By default, no logs from your EC2 instance will go to CloudWatch- we have to set it up

# Amazon EventBridge
• Schedule: Cron jobs (scheduled scripts)
• Event Pattern: Event rules to react to a service doing something
• Trigger Lambda functions, send SQS/SNS messages...

# AWS CloudTrail
• Provides governance, compliance and audit for your AWS Account
• CloudTrail is enabled by default!
• Get an history of events / API calls made within your AWS Account by:
• Console
• SDK
• CLI
• AWS Services

# AWS X-Ray advantages
• Troubleshooting performance (bottlenecks) • Understand dependencies in a microservice architecture • Pinpoint service issues • Review request behavior • Find errors and exceptions • Are we meeting time SLA? • Where I am throttled? • Identify users that are impacted

# Amazon CodeGuru
• An ML-powered service for automated code reviews and application performance recomendation

# AWS Personal Health Dashboard
• AWS Personal Health Dashboard provides alerts and remediation guidance when AWS is experiencing events that may impact you.
• While the Service Health Dashboard displays the general status of AWS services, Personal Health Dashboard gives you a personalized view into the performance and  availability of the AWS services underlying your AWS resources.
