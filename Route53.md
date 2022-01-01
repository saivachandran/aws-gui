* Route 53 is a managed Dns (domain name system)
* Dns is a collection of rules and records that help clients understand how to reach a server through urls.

* In Aws, the most common records are

   A:  url to ipv4 

   AAAA:  url to ipv6

   Alais: from one URL to another url

   CNAME: url to aws resource
   
# Route 53 Diagram

![image](https://user-images.githubusercontent.com/42309948/147843105-1c6ca62c-5fdc-4b7f-aaf3-7ddcc7aa71f2.png)


* route53 can use

  1. pubic doamin names own (buy)
  2. private domain resolve instance within vpc


* advance route53 options

  1. loadbalancing (throuh Dns client loadbalancing)
  2. Health check although limited
  3. Routing policy : simple, failover,geolocation, geoproximity,latency weighted

* prefer alias over cname to aws resources (for performance reasons)

