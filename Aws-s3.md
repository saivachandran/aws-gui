* Aws s3 allows people to store objects (files) in "buckets" .
* The bucket must have a globally unique name.
* Buckets are defined at the regional level.
* Naming converntion
   1. No uppercase
   2. No unerscore
   3. 3-63 character long
   4. Not an ip
   5. must start with lowecaseletter or number
   
* object (file) have key, key is fullpath
* Maximum size is 5Tb   
* if uploading morethan 5Gb use multipart upload

# create s3 bucket creation process

   1. s3 Dashboard
 
      ![image](https://user-images.githubusercontent.com/42309948/148335850-b2342c0c-2fab-45ac-92a9-23b08d4cd729.png)
      
       
   
   2. create s3 bucket

      ![image](https://user-images.githubusercontent.com/42309948/148335976-28afb97f-8cc1-41f6-906d-607d61f8e8c4.png)

  
  4. upload file inside s3 bucket
  
     ![image](https://user-images.githubusercontent.com/42309948/148336501-de25893f-05fb-48b8-8631-4959a9656776.png)
     
     ![image](https://user-images.githubusercontent.com/42309948/148336681-3b491797-6a62-4065-9b8b-ef8af5ec850f.png)
     
     
     ![image](https://user-images.githubusercontent.com/42309948/148336944-f66615e8-ce8b-4b9e-83d8-4cf18fae9878.png)
     
     
# aws s3 versioning

1. you can version your file in aws s3
2. it's enabled at bucket level
3. same key overwrite will increment version 1,2,3
4. it's best practice version your buckets
5. protect from iunintended deletes
6. Easy rollback to previous version

# Enable versioning

![image](https://user-images.githubusercontent.com/42309948/148344324-75badd9b-7e92-4d65-b12c-942e1736ce44.png)

![image](https://user-images.githubusercontent.com/42309948/148344429-7a40279d-3d67-4441-9972-89ce79f02ffa.png)

  1. upload same file multiple times it enable versioning for that file

![image](https://user-images.githubusercontent.com/42309948/148344644-8417521a-a3f4-4d12-9263-10848de0f70d.png)


# s3 encryption for objects

   1. SSE-S3 encrypt s3 object using key handled managed by aws
   2. SSE-KMS aws key mangement service 
   3. SSE-C you want to mange own encryption key
   4. client side encryption

# Enable s3 bucket default encryption

![image](https://user-images.githubusercontent.com/42309948/148362396-d7fde3f4-94da-4c7f-b04c-53e55d93d39f.png)

# s3 security

* user based
   
   1. IAM policies -which Api calls should be allowd  for as specific user from IAM console
   
* Resource based
   1. Bucket policeis - bucket wide rules from s3 console -allow cross account
   2. Object access control list - finer grain
   3. Bucket Access control list - less common   

* s3 bucket policy
  * json based polices
     
     1. Resources - buckets and objects
     2. Actions - Set of Api Allow or deny
     3. Effect - Allow or deny
     4. principle - The account or user apply the policy to

* use s3 bucket ploicy to
 
  1.Grant public Access to the bucket
  2. force object encryped at upload
  3. Grant access to another account (cross account)
  
  


   
 



  
   
    
  
 
  
  


     
  



  



     
      
   
   
   
       

   


    
   
   
   
   

