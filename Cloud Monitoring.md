# CloudWatch matrix

• CloudWatch provides metrics for every services in AWS
• Metric is a variable to monitor (CPUUtilization, NetworkIn...)

got o cloudwatch service-
![image](https://user-images.githubusercontent.com/107784718/213375955-cc46424f-7aa2-437f-be76-c1ffacf2b984.png)

got to all metrics an dselect any service to view the health of the respective
![image](https://user-images.githubusercontent.com/107784718/213376394-cfc1e998-dba5-42aa-8d46-cb53306dbddb.png)

To create an alarm:
Alarms-all alarms-create alarm- select metrics-select any service(example EC2)-select pre-instance metrics-let's do it for CPUUtilization- 
![image](https://user-images.githubusercontent.com/107784718/213376691-c7405350-9868-4bef-bef0-2754e221396d.png)

![image](https://user-images.githubusercontent.com/107784718/213376764-af3992c0-978b-42a5-bc3f-641074af1876.png)
![image](https://user-images.githubusercontent.com/107784718/213376816-4ae11664-5fb8-4288-a0ad-98db11a6c555.png)
![image](https://user-images.githubusercontent.com/107784718/213376870-533cfa33-97f9-4dc4-a10e-be43193c5294.png)
![image](https://user-images.githubusercontent.com/107784718/213376924-00727382-0d1f-46c5-a126-30cc12f6f7b6.png)
![image](https://user-images.githubusercontent.com/107784718/213377067-6f0f0a70-4f7c-4f2a-abdb-3eee17624810.png)

Metric- set period for which you have to trigger alarm
conditions-define threshold value- Next
![image](https://user-images.githubusercontent.com/107784718/213377476-9ed56365-943d-47f3-aaa6-5dbad74d7cb0.png)

![image](https://user-images.githubusercontent.com/107784718/213377537-9d01257e-7892-441d-873a-5ecba3c03bdf.png)
set up notifications for your emial- next
name- next
![image](https://user-images.githubusercontent.com/107784718/213378037-38e7f70a-ac55-4897-8af3-95ce4e9f9a0d.png)
preview the data an dlcik on craete alarm

We can create alarm directly from EC2 instance-
go to your instance- scroll right on your selected instance- alarm status- click on + icon- now you can setup your alarm for EC2 instance
![image](https://user-images.githubusercontent.com/107784718/213378619-46f1af42-0a56-41d8-9948-4a43d27a32a3.png)
select the craeted alarm- update
alarm action- recover- to recover the instance if value is gretaer then threshold, we can reboot, recover, stop or terminate the instances
![image](https://user-images.githubusercontent.com/107784718/213378892-bae7ee08-7711-4666-b7bf-6563ab6f35fa.png)
![image](https://user-images.githubusercontent.com/107784718/213378932-9526c12b-584d-40f8-975e-2a2d671efd34.png)
![image](https://user-images.githubusercontent.com/107784718/213378969-97a92e95-0732-4867-8af2-69f933d006fb.png)



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
