<h2>  ECS cluster</h2>

 * A logical grouping of EC2 instances It's known as the ECS cluster.
 * The ECS instances run the ECS agent (a Docker container).
 * The Ecs agent registers the instance with the ECs cluster.
 * The ECS instances run a special AMI, made especially for ECS.


<h2> Flow chart <h2/>
  
  ![image](https://user-images.githubusercontent.com/42309948/146877472-30c872e8-2880-4c22-8209-cd4ff0728cdc.png)

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

 # steps 1.2
  
     * provide cluster name
     * give provisional model (On demand instance)
     * instance type (t2.micro)
     * Number of instance (as you required)
     * Ec2 AMi id (Ecs Ami comes with docker installed on it)
     * EBS volume size (30)
     * key pair (Your key)
     * vpc (Defult vpc)
     *  subnet (Three subnets)
     * create security group with rule
     * container instance iam role
     * click create
  
     
  
  
  
  
  
  
                    

  
  
  
  
  
  
  

  
