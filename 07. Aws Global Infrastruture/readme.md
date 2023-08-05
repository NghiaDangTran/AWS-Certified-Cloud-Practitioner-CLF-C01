![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/58a053c0-8d17-4abc-85a6-7e34913eabed)
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/66d368fc-e7c9-4a8f-8ba3-b2a98d83f880)


# Why global
 - a global APP, is a app that deployed in multiple geographies
 - this could be region and or edge locations
 - decreaased latency
 - disater recovery
 - attack protection
     - regions: for deploying app and infrastructure
     - Availability Zone: made of mutiple data center
     - edge location: loaction to cached data

# AWS Route 53
 - managed DNS(domain Name System)
     - map from a string to a IPv4
     - ipv6
     - CNAME: hostname to hostname
     - AWS resource== ALias
 - simple routing policy (no heath check)
     - like u enter domain name Route53 return the ip
 - weighted routing policy
     - set each instance a %
 - latency routing policy
     - get the lowest latency for user
 - failover routing
     - check the fail server, and send to the healthy one
# CloudFront
 - imporces read performace, content is cached at edage
 - DDOS protection, intergration with Shield,
   - s3 bucket
   - for distributing  files and chacing them
   - OAC
 - Custom origin
     - Application load balancer
     - ec2 intance
     - s3 website
     - any http backend u want
 ## cloud front vs s3 cross region replication
  - cloudfront: global edge network, files are cached
  - good for static content
 ## s3  cross region replication
  - only copy ur data from one bucket to another bucket, so each time use need to grap that file again
# s3 transfer acceleration
 - tranfer data to s3 by using edge location
# golobal accelerator
 - ipromve global application availbility
 - by using edge location,
 - user only need to connect to edge location from there it use private aws internet to get data from our server
different with cloud front is taht it will cache the image or video, this is not 
# AWS outpost
 - they build the rack for u, but u must handel the outpost rack security
 - low latency,access to on peremisse system
 - local data processing
# AWS WaveLength
 - ring aws service to the edge of the 5G network
 - ultra low latency though 5g network
 - mainly just for application that need ultra low latency
# Aws Local Zones
 - extend your VPC to more location
 - extionsion of an aws
 - like one region have AZ a, AZB
 - but in each region the have local zaones, city a, city b city c
# global applicaion architecture
 - single region, single AZ (low abailablility, slow latency, easy to setup)
 - single region, mutile az, availability is high, slow latenct (meium setup)
 - multi region, acitve-passive (one main region support reaad write, one passive support read only) fast read but slow write, medim setup
 - multi region, active -active, both have read write, hard to do
