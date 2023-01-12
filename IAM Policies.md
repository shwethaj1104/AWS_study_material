
IAM user with admin privilage can see the list of users if he don't have admin previlage he will not be able to see te user.
remove user from the IAM group-
![image](https://user-images.githubusercontent.com/107784718/212034721-33425dae-ee8b-4043-ac03-8c911ab5c16c.png)

once the user is successfully removed from the group- if ypu try to check the list of users from that particular user account you will get an error
![image](https://user-images.githubusercontent.com/107784718/212035000-db7f3e70-2d36-4ae0-9bbf-ba8b35a0a238.png)

you can make it as earlier using 2 ways-
1. go to users and select ur IAM user and add amin policy
2. go to user groups and add your IAM user to it
