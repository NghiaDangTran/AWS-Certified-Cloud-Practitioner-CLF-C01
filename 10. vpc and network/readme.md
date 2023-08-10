![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/09dc2682-7b75-40b0-9dfc-55a56b375304)
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/0465a929-12d3-4894-b41c-bb28a6df900d)

# IP address in AWs
 - IPv4 -32 bit
     - ec2 instanace gets a new ip everytime u stop and then start
     - private ipv4 - can be use on private network (LAn) such as internal AWS network- fixed even if u start/stop
 - elastic IP
     - allows u to attach a fixed public ipv4 to ec2
     - has ongoing if not attached to ec2 or if the ec2 is stopeed
 - IPv6 -128 bit
     - ecery IP addresss is public
# VPC and Subnets Primer
 - VPC - virtual private cloud: regional resuorce
 - subnets, allow u to partition your network inside your VPC (AZ resource)
 - a public subnet is a subnet that is accessible from the internet
 - a private subnet not accessible from internet
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/55647eb5-6835-4092-a286-ae2036b359be)
 - to define access to the internet and btw subnets, we need `Route Tables`
# internet GateWay and NAT gateways
 - internet gateway (IGW) connect public subnet within a AZ to the outside internet
 - NAT Gateway (NAT) connect privte subnets to the internet
# networl ACL and Security Groups
 - NACl is network acl
     - a fire wall which controls traffic from and to subnet
     - con havve allow and deny
     - are attached at the `subnet` level
     - rules only indcldue ip address
 - Security Groups
    - a firewall that controls traffict to and from ec2
    - only have `allow`
    - rule in ip address and orther security group
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/d6902f93-c900-4285-9729-561b439fa490)
# VPC Flow Logs
 - capture information about IP traffic going into ur interface
 - vpc flow ,logs
 - subnets
 - elastic network interface
    - debung connectivity
       - subnets to internet
       - subnets to sub nets
       - internet to subnets
 - save network logs from ELB, ELAStce cache, EDS, AUrora
 - save s3,
# VPC Peering
 - connect 2 VPC, privately using network
 - make them behave as if they were in the same network
 - must have different CIDR
 - vpc connection is not transitive, (A->B, b->c ,A not to c)
# VPC Endpoints
 - allow u to connect to AWS service using a private network
 - better security and lower latecny to aws
 - vpc endpoint Gateway: S3 and Dynamo DB
 - vpc endpoint interfacce-> connect the rest
# AWS PrivateLink
 - most secure and scable way to expose service to 100s vps
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/6ddcfe8d-11fe-4667-b297-9c2e86ea0b1b)
# Direct Connect and site to site vpn
 - site to site -> use vpn to connect ( use customer gate way and vitual private gateway to connect)
 - Direct Connection -> establish physcall connection btw, on premises and AWS, private network
# Client VPN
 - connect from ur pc using Open VPN to ur private network
 - goes over public internet
# Transit Gate way
 - for having transitive peering btw thousad of vps and on premis and hub and spoke star connection
 - keys 1000s vpc and also on premise network
