# EBS Snapshots

    • Make a backup (snapshot) of your EBS volume at a point in time
  
  • Not necessary to detach volume to do snapshot, but recommended
  
  • Can copy snapshots across AZ or Region

How to make snapshots?

Go to volumes- select any volume- actions- create snapshot- add description- click create snapshots
![image](https://user-images.githubusercontent.com/107784718/212531564-e7d068a2-c6eb-449e-b160-8fe44bf407a1.png)

![image](https://user-images.githubusercontent.com/107784718/212531619-fa4a51b6-6174-4923-b76a-db83b7134684.png)

we can now copy the snapshots in to any AZ
right click on snapshot- copy snapshot- select the region 
![image](https://user-images.githubusercontent.com/107784718/212531645-6d5bd3d5-2012-48fd-aa0d-292d588cbe51.png)

we can re raete volume from the snapshot too
select snapshot- action- create volume from snapshot- give details and any AZ - Create volume

we also have recycle bin to avoid accsidental deletions of snapshots

![image](https://user-images.githubusercontent.com/107784718/212531815-071062a5-c3bb-4ccf-a5cb-d42aadc81564.png)

we can create retention rules to recover the snapshots after x number fo days after deletign them

![image](https://user-images.githubusercontent.com/107784718/212531833-ea0efd98-f21d-473e-9a4f-81329a648714.png)

![image](https://user-images.githubusercontent.com/107784718/212531848-34b8d1c0-516d-4588-8441-98419edf2fe2.png)
