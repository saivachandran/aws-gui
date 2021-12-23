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

  


 

