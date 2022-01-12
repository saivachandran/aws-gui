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
*  
