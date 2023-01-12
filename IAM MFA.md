MFA - Multi factor authentication

• Users have access to your account and can possibly change configurations or delete resources in your AWS account
• You want to protect your Root Accounts and IAM users

• MFA = password you know + security device you own

Account settings- chnage password policy-
set password policy as per you require- save chnages

MFA will be for root account
click on ur account- security credentials- activate MFA
![image](https://user-images.githubusercontent.com/107784718/212045461-07bb3f0c-4894-4d03-8925-6ebe6f842aae.png)

There are 3 options for MFA devices-
•virtual MFA device- mobile
•U2F security key-YubiKey or other
•other hardware MFA devices-Gemalto token


There are also 3 compatible apps you can setup with- install virtyual MFA applications- check for andriod or Apple devices apps- recommended to use Authy
scan the code in phone and 2 codes will be genrated with time lapse of 15 seconds, so give them - assign MFA
