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
