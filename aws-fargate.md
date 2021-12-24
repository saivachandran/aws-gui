* When we create an ECS cluster, we have to launch EC2 instances.
* If we need to scale, we have to add EC2 instances.  
* So we manage infrastructure.
* With Fargate, it's all serverless.
* We don't provision EC2 instances.
* We just create a task definition. AWS will run a container for us.
* To scale, just increase the number of tasks, no more EC2 instances.

# step 1

![image](https://user-images.githubusercontent.com/42309948/147352973-5a4f50c3-44b4-43e8-9b35-4923a8d40552.png)

# step 2

![image](https://user-images.githubusercontent.com/42309948/147353084-14413e93-f75e-4803-8ced-e9ca8de70b2a.png)

# step 3

![image](https://user-images.githubusercontent.com/42309948/147353200-57c22b85-dc61-4905-882d-96583839629d.png)

# step 4 create task definition

![image](https://user-images.githubusercontent.com/42309948/147353277-9ed0cfe2-96cf-4c6c-9928-8bfae6e61a31.png)

# step 5 select launch type template

![image](https://user-images.githubusercontent.com/42309948/147353555-c0503057-1f9f-44fb-b3ec-da9feabef53f.png)

# step 6 configure task and container section

![image](https://user-images.githubusercontent.com/42309948/147353777-3422e125-81e2-45b9-b2e6-ac5725869923.png)

# step 7 Add container section

![image](https://user-images.githubusercontent.com/42309948/147354476-29a6cd77-c303-471b-bc98-6f4c33975d4a.png)

  * create task definition.

# step 7  create service

![image](https://user-images.githubusercontent.com/42309948/147354610-3b3b89ed-0f90-4ddb-b8b1-b0507b8ce267.png)

# step 8 service next window

![image](https://user-images.githubusercontent.com/42309948/147354753-b79264ef-036b-4998-8f52-adbfe3023dc1.png)

# step 9 service next window

![image](https://user-images.githubusercontent.com/42309948/147355003-43848cbb-d63a-45cb-bcd6-ab7280c9d3b3.png)

# step 9 autoscaling optional not required here

![image](https://user-images.githubusercontent.com/42309948/147355097-97471b95-95f2-4e1d-8b22-599679b39381.png)

# step 10 Review and create service

![image](https://user-images.githubusercontent.com/42309948/147355154-5c0eea03-6c69-45c2-b2cf-2e475e7b5bd6.png)

# fargate Dashboard

![image](https://user-images.githubusercontent.com/42309948/147355300-36ccc274-3e60-475f-9475-446ecea08cef.png)

# Access via the alb url

![image](https://user-images.githubusercontent.com/42309948/147355419-0307bd00-c827-4960-8d20-4bf7032c98b5.png)

   * Before creating a service in Fargate, we need to create a load balancer.



















