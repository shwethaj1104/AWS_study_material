EBS Volume

    • An EBS (Elastic Block Store) Volume is a network drive you can attach to your instances while they run

    • It allows your instances to persist data, even after their termination

    • They can only be mounted to one instance at a time (at the CCP level)

    • They are bound to a specific availability zone

    • Controls the EBS behaviour when an EC2 instance terminates

    • By default, the root EBS volume is deleted (attribute enabled)

    • By default, any other attached EBS volume is not deleted (attribute disabled)

select EC2 instance - storage-you will be able to see the block storage for that instance
![image](https://user-images.githubusercontent.com/107784718/212531076-1b38dbd0-d46e-42cb-becd-b743eaba7e1e.png)


To craete new volume:
Elastic block store- volumes-create volume -give type- size-availability zone must be same as EC2 instance zone to attach for that isntance- create vlume
![image](https://user-images.githubusercontent.com/107784718/212531139-d0d3e894-8a1f-4409-bb58-7ded1ca9cdcd.png)

To attach volume to EC2 instance:
Select craete volume- Actions- attach volume

![image](https://user-images.githubusercontent.com/107784718/212531229-88a8deab-ce2b-4e6b-9d74-02eef786d78f.png)
![image](https://user-images.githubusercontent.com/107784718/212531242-e8b750c2-f0ad-4e05-b706-745a6de2d330.png)
click on attach volume

Now if you check in your instance you will be having 2 instances attached
![image](https://user-images.githubusercontent.com/107784718/212531279-591e2c00-2a89-489c-8a8e-135f153df9db.png)

if we terminate instance the root volume will be deleted and other volume which was attached wil be freed up so that we can use/attach it for other instances
