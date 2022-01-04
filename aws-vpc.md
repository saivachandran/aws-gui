* In a region, you are able to create a vpc (Virtual private cloud).
* Each VPC contains subnets (networks).
* Each subnet is mapped to AZ.
* It's common for public subnets to have public IPs.
* It's common for private subnets to have private IPs.

# vpc Diagram

![image](https://user-images.githubusercontent.com/42309948/148034555-cbfb57d4-bb63-45f8-9289-9ed8e0fb6d37.png)

# step 1 create vpc

![image](https://user-images.githubusercontent.com/42309948/148042207-d83481a5-c28b-44c7-8dc1-5e0877e1e3da.png)

# step 2 create pub-subnet

![image](https://user-images.githubusercontent.com/42309948/148042845-b48848da-bb3b-4311-b145-eab808357a41.png)

# step 3 create pri-subnet

![image](https://user-images.githubusercontent.com/42309948/148043218-307e22d7-a152-4b73-b7b1-98c5f7a6d10a.png)

# step 4 create pub-routetable

![image](https://user-images.githubusercontent.com/42309948/148043526-5a944f90-a1fe-4e77-a83a-01922ac03597.png)

# step 5 create pri-routetable

![image](https://user-images.githubusercontent.com/42309948/148043877-f1047588-1f4a-4d6d-a311-f8532ca35211.png)

# step 6 create internet gateway attach to vpc

![image](https://user-images.githubusercontent.com/42309948/148044295-30be4d21-58cc-42a3-889a-e71ad373b27b.png)

![image](https://user-images.githubusercontent.com/42309948/148044556-d0d45283-8647-4dfc-a863-b2509c553cbf.png)

![image](https://user-images.githubusercontent.com/42309948/148044647-6d9ade72-59ad-4f74-be9c-1154e51abc33.png)


# step 7 Create natgateway 

![image](https://user-images.githubusercontent.com/42309948/148046149-8ca4e86b-4e47-46f7-9e71-acdb00cc2404.png)

# step 8 Associate subnet

![image](https://user-images.githubusercontent.com/42309948/148051499-ea462c30-2f40-4518-b6fd-bceeab9d765a.png)

![image](https://user-images.githubusercontent.com/42309948/148054831-30d29d60-a83d-4204-941b-528d10df6c7a.png)

![image](https://user-images.githubusercontent.com/42309948/148056626-9d6ccfa7-6f3d-4dd4-a648-6f789593968a.png)


![image](https://user-images.githubusercontent.com/42309948/148055111-bfc46a80-e565-4897-8570-b63954f2fdf8.png)

# step 9 select rt edit route add igw and nat gateway

![image](https://user-images.githubusercontent.com/42309948/148055368-073e4b14-b84e-42ec-b228-38d8a8ef7722.png)

![image](https://user-images.githubusercontent.com/42309948/148055514-ad1b2ff3-f06d-4d3d-bc19-7250b800bc05.png)


![image](https://user-images.githubusercontent.com/42309948/148056470-2b9500ac-55a9-4ad0-a33f-4b4b0827613f.png)


![image](https://user-images.githubusercontent.com/42309948/148056146-91359063-8096-4534-ac98-b26431149951.png)




















