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

# step 1 create loadbalancer

![image](https://user-images.githubusercontent.com/42309948/147530815-d8d55b6a-b5f4-4b51-9d43-00d86376647e.png)


# step 2 select loadbalancer type


![image](https://user-images.githubusercontent.com/42309948/147469230-256b6a93-f314-4b7b-afea-dad59ec2719d.png)

 
 # step 3 create Application loadbalancer
 
 ![image](https://user-images.githubusercontent.com/42309948/147531343-f980def6-abc3-4fd1-b2ae-0648eca60d6b.png)

# step 4 create target group

![image](https://user-images.githubusercontent.com/42309948/147531529-04b8c72a-53e7-4936-8418-54e3576bef47.png)

# step 5 Target group next window

![image](https://user-images.githubusercontent.com/42309948/147531717-eef184c9-1721-431a-8d90-d2903c4fe71e.png)

# step 6 loadbalancer dashboard

![image](https://user-images.githubusercontent.com/42309948/147532340-de3de8a9-822c-4e5a-a76e-8d92dc4f40e9.png)


