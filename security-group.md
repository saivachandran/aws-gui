# security group in aws
Security group act as firewall for ec2 instances

1.security group funtamental network security in aws

2.They control how traffic allowd in to ec2 machines

# flow chart

![image](https://user-images.githubusercontent.com/42309948/146674283-f8713080-93eb-452b-9223-504bcf7ab7c2.png)

# security group

![image](https://user-images.githubusercontent.com/42309948/146674398-0ce4db44-49dc-46e7-a839-8df0e8142375.png)

1. inbound rule

Inbound rules control the incoming traffic to your instance,

2. outbound 

 outbound rules control the outgoing traffic from your instance. When you launch an instance, you can specify one or more security groups. If you don't specify a security group, Amazon EC2 uses the default security group.


# if we remove inbound rule, we won't ssh into ec2 machine

![image](https://user-images.githubusercontent.com/42309948/146674634-d830b625-6b33-4521-a382-a0526da4a939.png)


it show timedout error



