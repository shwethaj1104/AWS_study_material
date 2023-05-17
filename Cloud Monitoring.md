# CloudWatch matrix

• CloudWatch provides metrics for every service in AWS

• Metric is a variable to monitor (CPUUtilization, NetworkIn etc)

Go to cloudwatch service ->
![image](https://user-images.githubusercontent.com/107784718/213375955-cc46424f-7aa2-437f-be76-c1ffacf2b984.png)

Go to all metrics and select any service to view health of respective service ->
![image](https://user-images.githubusercontent.com/107784718/213376394-cfc1e998-dba5-42aa-8d46-cb53306dbddb.png)

To create an alarm :
Alarms -> All alarms -> Create alarm -> Select metrics -> Select any service(example EC2) -> Select pre-instance metrics -> Let's do it for CPU Utilization -> 
![image](https://user-images.githubusercontent.com/107784718/213376691-c7405350-9868-4bef-bef0-2754e221396d.png)
![image](https://user-images.githubusercontent.com/107784718/213376764-af3992c0-978b-42a5-bc3f-641074af1876.png)
![image](https://user-images.githubusercontent.com/107784718/213376816-4ae11664-5fb8-4288-a0ad-98db11a6c555.png)
![image](https://user-images.githubusercontent.com/107784718/213376870-533cfa33-97f9-4dc4-a10e-be43193c5294.png)
![image](https://user-images.githubusercontent.com/107784718/213376924-00727382-0d1f-46c5-a126-30cc12f6f7b6.png)
![image](https://user-images.githubusercontent.com/107784718/213377067-6f0f0a70-4f7c-4f2a-abdb-3eee17624810.png)

Metric -> Set period for which you have to trigger alarm
Conditions -> Define threshold value -> Next
![image](https://user-images.githubusercontent.com/107784718/213377476-9ed56365-943d-47f3-aaa6-5dbad74d7cb0.png)
![image](https://user-images.githubusercontent.com/107784718/213377537-9d01257e-7892-441d-873a-5ecba3c03bdf.png)

Set up notifications for your emial -> Next
Name -> Next
![image](https://user-images.githubusercontent.com/107784718/213378037-38e7f70a-ac55-4897-8af3-95ce4e9f9a0d.png)
Preview the data and click on create alarm.

We can create alarm directly from EC2 instance ->
Go to your instance -> Scroll right on your selected instance -> Alarm status -> Click on + icon -> Now you can setup your alarm for EC2 instance.
![image](https://user-images.githubusercontent.com/107784718/213378619-46f1af42-0a56-41d8-9948-4a43d27a32a3.png)
Select the created alarm -> Update

Alarm action -> Recover -> To recover the instance if value is greater then threshold, we can reboot, recover, stop or terminate the instances.

![image](https://user-images.githubusercontent.com/107784718/213378892-bae7ee08-7711-4666-b7bf-6563ab6f35fa.png)
![image](https://user-images.githubusercontent.com/107784718/213378932-9526c12b-584d-40f8-975e-2a2d671efd34.png)
![image](https://user-images.githubusercontent.com/107784718/213378969-97a92e95-0732-4867-8af2-69f933d006fb.png)

Billing alarm is available only for us-east-1 -> Create alarm ->
![image](https://user-images.githubusercontent.com/107784718/213379588-92a87c7b-d0c2-4c28-9491-d9638e8a14c4.png)
![image](https://user-images.githubusercontent.com/107784718/213379720-bfb89730-a971-4896-957c-792fe960b9f6.png)
![image](https://user-images.githubusercontent.com/107784718/213379728-4e0cd65f-4c3f-487d-b35e-87b37f6d9ecd.png)

# Important Metrics

• EC2 instances : CPU Utilization, Status Checks, Network (not RAM)

• Default metrics every 5 minutes

• Option for Detailed Monitoring ($$$) : metrics every 1 minute

• EBS volumes : Disk Read/Writes

• S3 buckets : BucketSizeBytes, NumberOfObjects, AllRequests

• Billing : Total Estimated Charge (only in us-east-1)

• Service Limits : how much you’ve been using a service API

• Custom metrics : push your own metrics

# Amazon CloudWatch Alarms

• Alarms are used to trigger notifications for any metric

• Alarms actions...

• Auto Scaling: increase or decrease EC2 instances “desired” count

• EC2 Actions : stop, terminate, reboot or recover an EC2 instance

• SNS notifications : send a notification into an SNS topic

# Amazon CloudWatch Logs
• CloudWatch Logs can collect log from :

• Elastic Beanstalk: collection of logs from application

• ECS: collection from containers

• AWS Lambda: collection from function logs 

• CloudTrail based on filter 

• CloudWatch log agents: on EC2 machines or on-premises servers

• Route 53- log DNS queries

• By default, no logs from your EC2 instance will go to CloudWatch- we have to set it up
_______________________________
What ever our application will be logging will be available here
![image](https://user-images.githubusercontent.com/107784718/213381413-682f1612-b254-46ed-a45b-9721c3f10509.png)

# Amazon EventBridge
• Schedule: Cron jobs (scheduled scripts)

• Event Pattern: Event rules to react to a service doing something, send notifications etc

• Trigger/invoke Lambda functions, send SQS/SNS messages...
___________________________

Select amazon event Bridge service -> Create rule -> Name -> Schedule -> Continue -> Give schedule pattern -> Next -> Select target(invoking lambda function/notig=fication for login on console/ notification on EC2 instance state chnage etc)

![image](https://user-images.githubusercontent.com/107784718/213383988-1d571f77-a6e2-4f21-b9e0-07604cd3c8a5.png)
![image](https://user-images.githubusercontent.com/107784718/213384069-e1a18ad9-6da0-453b-bb0c-467121745966.png)
![image](https://user-images.githubusercontent.com/107784718/213384259-6f446835-88ef-46c7-823e-1ddda049aed3.png)

# AWS CloudTrail
• Provides governance, compliance and audit for your AWS Account

• CloudTrail is enabled by default!

• Get an history of events / API calls made within your AWS Account by:

    • Console
    
    • SDK
    
    • CLI
    
    • AWS Services
___________________________
Select cloudTrial service-Event history -> what ever actions ahs been performed will be recorded in cloudTrial
![image](https://user-images.githubusercontent.com/107784718/213385193-439fd716-097e-427d-bcfd-4da159b4fafd.png)

# AWS X-Ray advantages
• Troubleshooting performance (bottlenecks) 

• Understand dependencies in a microservice architecture 

• Pinpoint service issues 

• Review request behavior 

• Find errors and exceptions 

• Are we meeting time SLA? 
• Where I am throttled? • Identify users that are impacted

# Amazon CodeGuru
• An ML-powered service for automated code reviews and application performance recomendation

# AWS Health Dashboard
# AWS Service Health Dashboard
 The Service Health Dashboard displays the general status of all AWS services
# AWS Personal Health Dashboard
• AWS Personal Health Dashboard provides alerts and remediation guidance when AWS is experiencing events that may impact you.
• Personal Health Dashboard gives you a personalized view into the performance and availability of the AWS services underlying your AWS resources.
__________
Bell icon- event log-
![image](https://user-images.githubusercontent.com/107784718/213385739-ba81c250-1660-4573-9989-c6a00c856466.png)
We can see the service health, personal account health etc
![image](https://user-images.githubusercontent.com/107784718/213386344-44c85bad-06ee-4f73-a724-3f1ed74ee8d4.png)


