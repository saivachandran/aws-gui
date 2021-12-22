<h2>  ECS cluster</h2>

 * A logical grouping of EC2 instances It's known as the ECS cluster.
 * The ECS instances run the ECS agent (a Docker container).
 * The Ecs agent registers the instance with the ECs cluster.
 * The ECS instances run a special AMI, made especially for ECS.


<h2> Flow chart <h2/>
  
![image](https://user-images.githubusercontent.com/42309948/147031202-bf8e91b4-e20f-4706-b167-80b39acebbcc.png)

<h2> ECS Dashboard <h2/>
  
  ![image](https://user-images.githubusercontent.com/42309948/146879171-287cc2b0-c332-4f51-a941-d8ce6a99b763.png)
  
<h2> create cluster<h2/>
  
  ![image](https://user-images.githubusercontent.com/42309948/146890436-21b11fe1-417c-40d5-b74f-bbbae7c6f22c.png)
  
<h2> select cluster template<h2/>
  
    
![image](https://user-images.githubusercontent.com/42309948/146892152-aba1905a-f95d-4ffb-9dd0-a5baf3e3baad.png)
  
#  step 1
  
     * Select Ec2 Linux + Networking from the three options.

     * Then, proceed by clicking on the next step.
  
 
 # step 1.1
  
  ![image](https://user-images.githubusercontent.com/42309948/146898507-139908ab-45f3-4426-898a-df6aac6501c0.png)

 # steps 1.1
  
     * provide cluster name
     * give provisional model (On demand instance)
     * instance type (t2.micro)
     * Number of instance (as you required)
     * Ec2 AMi id (Ecs Ami comes with docker installed on it)
     * EBS volume size (30)
     * key pair (Your key)
     * vpc (Defult vpc)
     * subnet (Three subnets)
     * create security group with rule
     * container instance iam role
     * click create
  
  
  # launch status
  
  ![image](https://user-images.githubusercontent.com/42309948/146902668-85ec8b1e-864b-4ffe-abb0-474889b6b3dc.png)
  
<h2> view cluster <h2/>
  
 ![image](https://user-images.githubusercontent.com/42309948/146908959-3bb9b007-1268-47f3-a96f-4d1c5be2999b.png)
  
  # Ecs cluster created with auto scaling group
  
      * When we create an ECS cluster, it comes with an autoscaling group.
      * Ec2 instance was created in the manner specified in the configuration section.
      * The security group was created and the ecs role was also created. That needs review after the cluster is created.
 
  
  ![image](https://user-images.githubusercontent.com/42309948/146921911-7fcdfe86-31d3-4f2d-ae00-01340bf9ab0b.png)
  
  # step 2 
  
      * ssh into our created EC2 instance using the instance public IP.
 
  ![image](https://user-images.githubusercontent.com/42309948/146923284-405d5591-0454-4b80-8e68-73fafbe8fa6f.png)
  
  # step 2.1
  
      ssh -i "key_name" username@publicip
      
      check cluster configuration
  
  ![image](https://user-images.githubusercontent.com/42309948/146926463-7b965942-edd8-48f1-827f-865d22d5a044.png)

 -------------------------------------------------------------------------------------------------------------------     
  
 # task 
    
      Task is JSON metadata that instructs ECs on how to run a Docker container.
  
       It contains crucial information about
  
          image name.

          port bindings for container and host
 
          Memory and CPU information.

          environment variables. 
  
          Networking information.
   
      
<h2> 1.create task definition<h2/>
  
![image](https://user-images.githubusercontent.com/42309948/147020199-2a91790b-7753-4a0a-a963-221c33c74444.png)
  
  # 2. Choose the launch type compatibility.
  
    
  ![image](https://user-images.githubusercontent.com/42309948/147020710-47906d1f-02ff-4d54-8588-5df981c4377d.png)
 
  
  # 3. configure task and container definition
  
 ![image](https://user-images.githubusercontent.com/42309948/147021048-9c44fbee-be50-4a25-947c-f8d6c9c11644.png)
  
  # 4. Add container section
  
 ![image](https://user-images.githubusercontent.com/42309948/147021559-63b2b0dd-44d3-4749-ba14-13ad4138ebd6.png)
   
    * if require we can configure advance option
  
    * click create
  
<h2> 1.service <h2/>
  
   * The Ecs service defines how many tasks should run and how they should run.
   * The Ecs service ensures the desired number of tasks running across the EC2 instances.
   * They can be linked to Elb and NLB, and ALB, respectively.
  
  # 2.Create service
  
  ![image](https://user-images.githubusercontent.com/42309948/147022747-38525f1b-e181-44c3-9f2b-6b9119e7c5b9.png)
  
  # 3. configure service
  
  ![image](https://user-images.githubusercontent.com/42309948/147023082-425d1414-2018-49b3-8891-c8a806003dab.png)
  
  # 4. configure Network
  
    * load balancer we can configure later
  
 ![image](https://user-images.githubusercontent.com/42309948/147023339-6a7555c0-dc53-4ad2-955c-c163ee4acf52.png)

  
  # 5. Autoscaling optional
  
  ![image](https://user-images.githubusercontent.com/42309948/147023510-87f0a9e4-88b2-4101-ba4e-7883dba492fb.png)

  
  # 6. Review and create service
  
  ![image](https://user-images.githubusercontent.com/42309948/147023614-a145ee12-18a1-4115-8cbf-e73e1f510379.png)
  
    * now task is running click container instance
    * Allow 8080 port in security group
    * if you want update task 1 to 2 scale autoscaling group it wil 2nd task
  
  # now ecs container launched now it's working
  
 ![image](https://user-images.githubusercontent.com/42309948/147029710-0e277a66-c647-4d14-a0e3-e3db41f4e014.png)

   
<h2> view running container <h2/>
  
![image](https://user-images.githubusercontent.com/42309948/147030213-2873f2bc-d7b7-4ab2-8d55-d6f5b6021dac.png)
  

<h2> change container image and configuration <h2/>
  
  # step 1
  
![image](https://user-images.githubusercontent.com/42309948/147094990-133235ee-7f2e-4f5b-9d1b-1ab693c3a6d1.png)
  
  # step 2
  
![image](https://user-images.githubusercontent.com/42309948/147095260-210f23c9-b3c8-41b3-8674-9a7020fb29a0.png)

  # step 3
  
![image](https://user-images.githubusercontent.com/42309948/147095604-83b8d78b-7bf5-4b78-aec3-ba31fff7d085.png)
  
  * update and create task
  
  # update cluster
  
 ![image](https://user-images.githubusercontent.com/42309948/147095861-f5849dc4-7d2f-4553-8d49-f849e3fc07cb.png)
  
  # select latest revision
  
![image](https://user-images.githubusercontent.com/42309948/147096054-89b7e577-72c8-48fa-bb20-42ff9619da89.png)

    * click next
    * click next
    * update service
  
 
  
  
  
  
  
  
  
  
  
  
  




  
  

  

  
  
  
  
  
  
  
                    

  
  
  
  
  
  
  

  
