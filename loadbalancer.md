# load balancer


Loadbalancer front in your application that traffic to multiple ec2 instances in downstream

# Flow chart

![image](https://user-images.githubusercontent.com/42309948/146756129-91f87cb6-effc-4835-a046-b30c15436974.png)

1. load balancer split the load across the downstream ec2 instances
2. do regular healthchecks of your instances
3. ssl termination for loadbalancer
4. high availablity across the zones
5. seperate public traffic from private traffic

# Types of load balancer

1. classic loadbalancer (v1 old generation 2009)
2. Application Loadbalancer(v2 new generation 2016)
3. network Loadbalancer(v2 new generation 2017)

overall it's recommended use v2 new generation loadbalancer they provide more features

# step 1 select loadbalancer type


![image](https://user-images.githubusercontent.com/42309948/147469230-256b6a93-f314-4b7b-afea-dad59ec2719d.png)
