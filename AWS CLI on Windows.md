Open AWS CLI install on windows- https://docs.aws.amazon.com/cli/latest/userguide/getting-started-version.html

Download windows 64 bit AWS CLI -> Install

Then open CLI -> Type -> "aws --version" to check which version is installed

![image](https://user-images.githubusercontent.com/107784718/212048159-10a2db43-0a61-4941-945d-01956f1634a5.png)

To upgrade AWS CLI version -> Just redownload the link and install it
______________________________________________________________________________________________________________________________________________________________
Your account name(top right section) -> Security credentials -> Create access key -> Download file or make note of secret key and access key.

Now open command promt from local computer -> "aws configure" -> Provide access key -> Provide secret key -> Provide region -> Enter for default output-- now it's all setup

To check type- "aws iam list-users"-> you will see all the users in your iam account.

To connect from cmd to ec2 instance:ssh -i ./tour-guider-keyPair.pem ec2-user@54.211.124.178
