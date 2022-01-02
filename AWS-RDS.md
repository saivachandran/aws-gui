# RDS is an abbreviation for Relational Database Service.
  
  1. Postgres
  2. Oracle
  3. mysql 
  4. mariadb
  5. Aurora
  6. Microsoft sql server

# RDS Advantages

 1. managed service
 2. Os patching level
 3. continous backup and restore on specific timestamp
 4. Monitoring Dashboard
 5. Read replicas for improved read performance
 6. multi Az setup for DR
 7. scaling capabilities
 8. But You can't ssh into your instances

# RDS Flowchart

![image](https://user-images.githubusercontent.com/42309948/147873078-11dbe3b8-5b8f-4617-9d2a-3a428326d9e7.png)

# step 1 create RDS Database

![image](https://user-images.githubusercontent.com/42309948/147876834-5eeaec15-0895-4dfb-864c-55f5d528f1ea.png)

# step 2 

![image](https://user-images.githubusercontent.com/42309948/147877155-bf7d32d6-3468-46bd-9207-b6720145e78b.png)

# stpe 3
  
  1. launch Ec2 instance an same availability zone
  2. install mysql client 

# stpe 4 

 1. ssh -i "Task.pem" ubuntu@ec2-52-51-61-185.eu-west-1.compute.amazonaws.com
 2. mysql -h mydb-1.ce6vulmtd00m.eu-west-1.rds.amazonaws.com -u techteam -p 
 3. use Bookstore;
 4.  4.CREATE TABLE Books ( id Int(3), Bookname Varchar (15), price Varchar(20), publishyear Varchar(20) ); 
 5.  INSERT INTO Books VALUES ('1' , 'Agnisiragukal' , '200' , '2020' );
 6.  select * from Books;
 
 
 
 

 




