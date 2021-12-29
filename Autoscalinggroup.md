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


# step 1 create Autoscalinggroup

![image](https://user-images.githubusercontent.com/42309948/147671815-a0ed9996-034f-40cc-9fcb-fd2fb00e6cce.png)

# step 2 create launch template for asg

![image](https://user-images.githubusercontent.com/42309948/147672325-0ee718d5-90a8-426e-b1a4-8a3e7426fbf6.png)

# step 3 Asg next window

![image](https://user-images.githubusercontent.com/42309948/147672726-3396c427-e9c7-4672-b3b3-a6c5c1fb66c2.png)

# step 4 Asg next window

![image](https://user-images.githubusercontent.com/42309948/147672993-ddfbd6ed-5c6a-4f2b-a2e5-941df5decb38.png)

# step 5 Asg next window

![image](https://user-images.githubusercontent.com/42309948/147673114-ef603738-8448-40a8-bc69-14e3590cf771.png)

# step 6 Asg next window

![image](https://user-images.githubusercontent.com/42309948/147673316-d8279c88-d11a-4044-be13-0cde557dfbd7.png)

# step 7 Asg next window

![image](https://user-images.githubusercontent.com/42309948/147673465-229e1495-f127-43e4-b88d-8f84da6fa766.png)

![image](https://user-images.githubusercontent.com/42309948/147673538-5730235a-291c-413a-a9f7-5fe21a3ac4ea.png)

# Review and create AsG

![image](https://user-images.githubusercontent.com/42309948/147673743-c7fcc860-ef8c-478e-8e24-e54e60d88727.png)


















    
