* Before we can use the loadbalancer, we must first create an Ecs cluster task and service.

# flow chart

![image](https://user-images.githubusercontent.com/42309948/147048579-e3a87a9c-b0a8-4253-b73c-12139925a4a0.png)
# step 1
![image](https://user-images.githubusercontent.com/42309948/147081055-04b623b1-86be-4b24-914d-f6ad5cd3bfb4.png)

  * create new revision using task defintion
  
  * Edit container section
![image](https://user-images.githubusercontent.com/42309948/147082102-b85752b3-90fb-487e-9e61-67583a06e647.png)

  * new task defintion created

# step 1: create service

![image](https://user-images.githubusercontent.com/42309948/147083368-974e29d0-9620-48c5-8557-32ff77ecd720.png)

# step 2 :

![image](https://user-images.githubusercontent.com/42309948/147084768-265c5f8a-be92-47ce-8303-5bfff11e2467.png)

# step 3:

![image](https://user-images.githubusercontent.com/42309948/147084874-e0e3dacf-d0bf-4723-84db-99cb6a2f368f.png)

# step 4: service status

![image](https://user-images.githubusercontent.com/42309948/147085054-d51fac7a-aad9-4914-b670-7a60654e1eb0.png)


# stpe 5 here we can see number of running tasks

![image](https://user-images.githubusercontent.com/42309948/147085435-32e87f56-46ad-4b62-8e36-d08cefedd983.png)

# step 6 checking running tasks in ec2 instance
 
   * first instance running 3 tasks
   * second instance running 3 tasks with dynamic port provision

![image](https://user-images.githubusercontent.com/42309948/147085886-833e8c71-0ba2-4cdc-9f3d-53c7e9140abc.png)

# check url with port number

curl localhost 49163



  





