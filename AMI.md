# AMI -> Amazon Machine Image
• AMI are a customization of an EC2 instance

• You add your own software, configuration, operating system, monitoring

• Faster boot / configuration time because all your software is pre-packaged

• AMI are built for a specific region (and can be copied across regions)
__________________________________________________
Create AMI ->

Select instance -> Actions -> Image and tempaltes -> Create image -> Provide description -> Click create image
![image](https://user-images.githubusercontent.com/107784718/212532418-cf877a31-50af-4aff-936c-430aa89f2ba8.png)

Go to images -> AMIs -> You can see your AMI there
____________________________________________________
To launch instances using AMI ->
instance- luanch instance- go to my AMI's tab- select your AMI from dropdown
![image](https://user-images.githubusercontent.com/107784718/212532475-56b89f3d-1ef4-4b64-a278-8305cfd0d8ef.png)

While writing user data- we just ahev to give what file to craete etc- since all the pre instalations have been done while creating AMI- basically we are reusing same AMI for faster boot time
