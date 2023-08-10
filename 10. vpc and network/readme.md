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
