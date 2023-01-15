
Open AWS CLI install on windows- https://docs.aws.amazon.com/cli/latest/userguide/getting-started-version.html

download windows 64 bit AWS CLI

Install

then open cli- type- aws --version to check which version is installed

![image](https://user-images.githubusercontent.com/107784718/212048159-10a2db43-0a61-4941-945d-01956f1634a5.png)

to upgrade aws cli versiob- just redownload the link and install it
______________________________________________________________________________________________________________________________________________________________
Users-security credentials- create access key- download file or make note of secret key and access key
![image](https://user-images.githubusercontent.com/107784718/212081168-b19cc107-99fc-4af4-acef-1d92eca55d73.png)

now open command promt from local computer- "aws configure"- provide access key- provide secret key- provide region- enter for default output-- now it's all setup

to check type- "aws iam list-users"-> u will see all the users in your iam account
