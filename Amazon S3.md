Amazon S3 Use cases

• Backup and storage

• Disaster Recovery 

• Archive 

• Hybrid Cloud storage 

• Application hosting 

• Media hosting 

• Data lakes & big data analytics 

• Software delivery 

• Static website

Amazon S3 - Buckets

• Amazon S3 allows people to store objects (files) in “buckets” (directories)
• Buckets must have a globally unique name (across all regions all accounts)
• Buckets are defined at the region level
• S3 looks like a global service but buckets are created in a region
• Naming convention
• No uppercase, No underscore
• 3-63 characters long
• Not an IP
• Must start with lowercase letter or number
• Must NOT start with the prefix xn--
• Must NOT end with the suffix -s3alias

________________________

AWS Snow Family

Highly-secure, portable devices to collect and process data at the edge, and migrate data into and out of AWS
___________
Snowball Edge (for data transfers)
 • Physical data transport solution: move TBs or PBs of data in or out of AWS

AWS Snowcone 
• Small, portable computing, anywhere. secure, withstands harsh environments
• Light (4.5 pounds, 2.1 kg) 
• Device used for edge computing, storage, and data transfer
• 8 TBs of usable storage
• Use Snowcone where Snowball does not fit(space-constrained environment)
• Must provide your own battery / cables • Can be sent back to AWS offline, or connect it to internet and use AWS DataSync to send data
________
AWS Snowmobile
• Transfer exabytes of data (1 EB = 1,000 PB = 1,000,000 TBs)
• Each Snowmobile has 100 PB of capacity (use multiple in parallel)
• High security: temperature controlled, GPS, 24/7 video surveillance
• Better than Snowball if you transfer more than 10 PB
______________
