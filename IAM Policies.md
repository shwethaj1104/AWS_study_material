
IAM user with admin privilage can see the list of users if he don't have admin previlage he will not be able to see te user.
remove user from the IAM group-
![image](https://user-images.githubusercontent.com/107784718/212034721-33425dae-ee8b-4043-ac03-8c911ab5c16c.png)

once the user is successfully removed from the group- if ypu try to check the list of users from that particular user account you will get an error
![image](https://user-images.githubusercontent.com/107784718/212035000-db7f3e70-2d36-4ae0-9bbf-ba8b35a0a238.png)

you can make it as earlier using 2 ways-
1. go to users and select ur IAM user and add existing policy-AdminReadOnly policy/administratorAccess

![image](https://user-images.githubusercontent.com/107784718/212036309-2736c066-f525-4c73-91b6-9704ab4ee1e6.png)

2. go to user groups and add your IAM user to it

now you can see which policies are added directly to users and which are from the groups
![image](https://user-images.githubusercontent.com/107784718/212036475-fe635bb4-5fec-4c3f-8fb6-3321d5592a38.png)

Go to policies and select any policy and we can check the access they have to
![image](https://user-images.githubusercontent.com/107784718/212037119-42772deb-17cc-40ed-9df2-cab147109f09.png)

we can even create our custom policy by clicking - create policy
![image](https://user-images.githubusercontent.com/107784718/212037613-1c3854f9-f338-42ff-8e32-d08511960512.png)

select the service policies and actions and resources and save it
![image](https://user-images.githubusercontent.com/107784718/212037950-0dbb9b9f-b3b9-4972-bead-d87caab89fed.png)
