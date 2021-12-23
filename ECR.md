* so for we are using images from dockerhub (public)
* ECR is aws private docker registry    
* Access control through IAM  (Permission error ==> policy)

# build your custom image

* sample dockerfile
* Dockefile content below
FROM nginx:latest

MAINTAINER Saiva

RUN ln -sf /dev/stdout /var/log/nginx/access.log
RUN ln -sf /dev/stderr /var/log/nginx/error.log

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]

# step 1

 * docker build -t my-nginx-image .

# create ECR repository on aws console

![image](https://user-images.githubusercontent.com/42309948/147207644-974bc23d-313c-4710-840c-5858eeda0872.png)

# step 2

![image](https://user-images.githubusercontent.com/42309948/147214957-da5f10c3-1368-48af-aec3-e238cd66d74d.png)

# repository dashboard view

![image](https://user-images.githubusercontent.com/42309948/147215151-4680f1ac-b248-46ac-9c8d-c47d969c69e3.png)



  * Go to inside into repository
  * Right side corner click view push commands

# repository commands

  1. get login

   aws ecr get-login-password --region eu-west-1 | docker login --username AWS --password-stdin 562399419057.dkr.ecr.eu-west-1.amazonaws.com
   
  2.  build image
   
     docker build -t demo1 .
     
  3. Tag image
  
    docker tag demo1:latest 562399419057.dkr.ecr.eu-west-1.amazonaws.com/demo1:latest   
    
  4. push image
  
    docker push 562399419057.dkr.ecr.eu-west-1.amazonaws.com/demo1:latest

 5. pull image

  docker push 562399419057.dkr.ecr.eu-west-1.amazonaws.com/demo1:latest
  
  
  # we need to give ECR path in task container section path looks like below
  
     562399419057.dkr.ecr.eu-west-1.amazonaws.com/demo1:latest



  


 

