# EC2 Setup


# Security Groups
 - control what go in and out of EC2
 - only cotain `allow` rule
 - can set by ip or security group
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/5b75052a-e4a0-4d61-910d-037575edc501)
  - regulate:
     - access to ports
     - authorised IP range Ipv4 and IPV6
     - control inbound network ( from orther to the instance)
     - contol outbound network (from instance to orther)
  ![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/9e4993f4-2cbe-49d4-b498-fd2f4de9262e)
 - can be attached to mutiple instances
 - `Locked` down to a` region`
 - should allow on `SSH port`
 - >if u cant accessible (highly it is security group issue)
### if the connection is `time out` then it is `security group issue`, when it is `connection refused` it is `application error or it's not running`
 - all inbound is `Blocked` by default
 - all outbound is `authorised` by default
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/fad53e5e-2ef4-4971-806b-dcadbbf400ef)
 - classic port to know
    - `22= SSH`
    - `21= FTP` upload files into a file share
    - `22 = sFTP` upload files using ssh
    - `80 = HTTP`
    - `443 = HTTPS`
    -  `3389 = RDP ` (Remote Desktop Protocol) log into a Windows instance 
