* To scale out (add EC2 instances) to match an increased load.
* scale in (remove EC2 instances) to match a decreased load.
* Make certain that we have a minimum and maximum number of machines running.
* Automattically register new instances with the loadbalancer.    

# Autoscaling group flowchart
![image](https://user-images.githubusercontent.com/42309948/147668642-1b893083-c614-499f-8c41-37435b847117.png)

# Asg with loadbalancer

![image](https://user-images.githubusercontent.com/42309948/147668761-14e7a691-7888-4405-b742-c18d75e0fae3.png)

# Asg have following attribute

 * Ami + Instance Type

 * User data

 * Ebs volumes

 * Security groups

 * ssh keypair

 * minimum, maximum, and desired capacity

 * Network and subnet information

 * loadbalancer information

 * Scaling policies







    