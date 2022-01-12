* SQS - standard queue service
* oldest offer over 10 years 
* fully managed
* scales from 1 messages per seconds to 1000 messages per second
* Default retention of messages 4 days, maximum 14 days
*  no limit how many messags in the queue
*  low latency (< 10 ms on publish and receive )
*  horizontal scaling interms of number of consumer
*  can have duplicate messages ( at least once delivery occasionaly ) 
*  limitation 256Kb size per message sent
*  don't send videos and big messages this not use case 
*  just sent small messages like json data
*  can Delay messages upto 15 minutes defult is 0
*  consumer pull messages from sqs

# SQS Flowchart

![image](https://user-images.githubusercontent.com/42309948/149077552-35fa9d9e-d8cf-468d-addb-badac16d0236.png)


# step 1

![image](https://user-images.githubusercontent.com/42309948/149082090-1b6a361b-9ac4-4d77-a886-8215627de765.png)


# step 2

![image](https://user-images.githubusercontent.com/42309948/149082426-df26d016-14a6-453c-b720-847fcb2d83ed.png)

# step 3

![image](https://user-images.githubusercontent.com/42309948/149082778-eed65989-0460-4bd5-a4db-4a2e4f25be34.png)

# step 4

![image](https://user-images.githubusercontent.com/42309948/149083036-7a9e2b0d-e4c3-4d85-b3d8-6c8d5e3bd9ba.png)


# step 4

![image](https://user-images.githubusercontent.com/42309948/149083241-56cfaac2-dff3-459a-a01b-8a9152926541.png)


# step 1 Dead letter queue

![image](https://user-images.githubusercontent.com/42309948/149086786-4cffdc1b-9f78-4b2c-8917-54fc0f6b53fe.png)

# step 2

![image](https://user-images.githubusercontent.com/42309948/149086933-92021a41-1d21-438f-bf2c-82f3a66a6097.png)

# step 3

![image](https://user-images.githubusercontent.com/42309948/149087061-4d799af4-26c7-409a-91b7-5e5c5741875e.png)

# step 4

![image](https://user-images.githubusercontent.com/42309948/149087305-c2736df7-c836-46b2-826e-07282802c761.png)

# step 4

![image](https://user-images.githubusercontent.com/42309948/149087611-d7d57259-49d6-4b55-bc3d-11e82bac2f31.png)

* after 3 un successfull recieves it will goes to Dlq queue


# Aws SQS - FIFO Queue

* Newer offering - Not available all regions 
* Name of the queue must end with .fifo
* Messages are processed by order
* Messages sent exactly one
* Deduplication can't sent same messages twice
* Deduplication interval is 5 minutes
* deduplication id is important


# step 1

![image](https://user-images.githubusercontent.com/42309948/149147402-89ece60f-ecfd-4022-9417-1f9f098b0069.png)


# step 2

![image](https://user-images.githubusercontent.com/42309948/149147650-4595452e-c94c-4add-b0ca-1ba49237348d.png)


* send message with same message id it's wont come in queue

# step 3 enable content duplication

![image](https://user-images.githubusercontent.com/42309948/149148459-8734d627-7970-4e81-97d6-24fdf7fc9afa.png)



















