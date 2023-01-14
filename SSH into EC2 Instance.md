SSH on windows-10

check whether you have SSH in your machine-cmd- type ssh-- if you see content lik below you are good to go with SSH else you need to use putty method

![image](https://user-images.githubusercontent.com/107784718/212467442-7c867359-42e4-432a-a78c-6aaa855c3bfd.png)

Go to folder path where your .pem file is-open cmd
Type ssh -i .\yourPEMFile.pem ec2-user@PublicIP
Meaning - entering the ip with the specified user, using provided pem key
