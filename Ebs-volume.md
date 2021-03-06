*   An Ec2 machine's root volume is lost when it's manually terminated.
*   Unexpected termination can occur at any time in the aws email you receive.
*   We sometimes need to store instance data somewhere.
*   An EBS (Elastic Block Store) volume is a network drive you can attach while your instance is running.
*   It allows your instance data to persist.
*   It's a network drive, not a physical drive.
*   It detached from one EC2 instance and attached to another instance very quickly.
*   It's locked to the availability zone volume, so us-east-1a can't attach to another region, us-east-1b.
*   To move the volume across, we first take a snapshot.
*   A snapshot can be used to backup an Ebs volume.  
*   snapshot take backup used space size 

# create two instance in differnet availabilty zones

![image](https://user-images.githubusercontent.com/42309948/147824414-311e8e10-1212-4eb5-ac13-f8b7f7b2a7cd.png)

# create volume one az eu-west-1a

![image](https://user-images.githubusercontent.com/42309948/147824849-5d877aa4-0709-4d3e-a521-e2058aac37d5.png)

# Attach volume with Ec2 instance 

![image](https://user-images.githubusercontent.com/42309948/147825939-5b3e603c-e8ff-4d18-9e10-d90334a2d873.png)

![image](https://user-images.githubusercontent.com/42309948/147826094-af3c9c6c-f631-49d5-94eb-4d78b07aa196.png)

# ssh into Ec2 machine check volume

![image](https://user-images.githubusercontent.com/42309948/147826379-f906cbaf-0c27-4074-8c12-b3905fcc0a03.png)

# format the volume

![image](https://user-images.githubusercontent.com/42309948/147826561-af379e05-4e4b-4672-9bde-24f2c35f0f03.png)

# mkdir and mount that volume

![image](https://user-images.githubusercontent.com/42309948/147826713-f3a9f7d8-7df4-4eaa-9141-ad69e17e891b.png)

# unmount and detach volume

![image](https://user-images.githubusercontent.com/42309948/147827138-8798038d-bdb0-4d90-b4a7-23fedec2efcb.png)

![image](https://user-images.githubusercontent.com/42309948/147827671-ad00f397-382a-446b-ae9c-84ecd0188085.png)

# to attach that volume to another AZ first take snapshot

![image](https://user-images.githubusercontent.com/42309948/147827840-9bb97107-46ed-4703-bf8a-e83f7637c0dc.png)

![image](https://user-images.githubusercontent.com/42309948/147828087-bcd42e7a-aa01-4959-91b2-24943ece4cad.png)

# create volume from that snapshot

![image](https://user-images.githubusercontent.com/42309948/147829550-e472ff0f-cea5-44b1-99f4-c1fc8ebaa824.png)

![image](https://user-images.githubusercontent.com/42309948/147829654-a2057321-6e44-453d-90e7-34c4d237264b.png)

# attach volume to anoth az ec2 instance

![image](https://user-images.githubusercontent.com/42309948/147829759-10a6b693-a594-4405-a880-550915a6ef94.png)

# mount and check the file is exist on the volume
















