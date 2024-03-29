# EBS Snapshots

    • Make a backup (snapshot) of your EBS volume at a point in time
  
    • Not necessary to detach volume to do snapshot, but recommended
  
    • Can copy snapshots across AZ or Region
____________________________________________________________________________________________________________________________________________________________________

How to make Snapshots?

Go to volumes -> Select any volume -> Actions -> Create snapshot -> Add description -> Click create snapshots
![image](https://user-images.githubusercontent.com/107784718/212531564-e7d068a2-c6eb-449e-b160-8fe44bf407a1.png)

![image](https://user-images.githubusercontent.com/107784718/212531619-fa4a51b6-6174-4923-b76a-db83b7134684.png)

We can now copy the snapshots in to any AZ.
Right click on snapshot -> Copy snapshot -> Select the region 
![image](https://user-images.githubusercontent.com/107784718/212531645-6d5bd3d5-2012-48fd-aa0d-292d588cbe51.png)

We can re create volume from the snapshot too
Select snapshot -> Action -> Create volume from snapshot -> Give details and any AZ -> Create volume

We also have recycle bin to avoid accsidental deletions of snapshots

![image](https://user-images.githubusercontent.com/107784718/212531815-071062a5-c3bb-4ccf-a5cb-d42aadc81564.png)

We can create retention rules to recover the snapshots after x number fo days after deletign them

![image](https://user-images.githubusercontent.com/107784718/212531833-ea0efd98-f21d-473e-9a4f-81329a648714.png)

![image](https://user-images.githubusercontent.com/107784718/212531848-34b8d1c0-516d-4588-8441-98419edf2fe2.png)
