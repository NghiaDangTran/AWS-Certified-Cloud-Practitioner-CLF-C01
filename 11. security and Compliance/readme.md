# AWS Shared Responsibility Model
 - AWS responsibility - security in Cloud
     - protecting infratstruc
     - managed service like s3, dynamoBD,RDS
 - User reponsibility - security in the cloud
     - for ec2 instance, customer reposible for managemnt of gust
     - encrypting data
 - shared controls:
     - patch management, configuration , awareness and trraing
 ![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/57c95550-f3f1-46e5-b9d0-727abb0d1159)

# DDOS Attack
 - AWS Sheild Standard: protact agasit DDOS
 - AWS Sheild Advanced: 24/7 DDos protection
 - AWS WAF: filter specific request based on rules
 - cloudFront and Route 53:
     - Availability protection using global edge network
     - combined with AWS Sheild, provides attack mitigration at the edge
     - AUto Scailing
# AWS Sheild
 - AWS sheild Standard:
     - free service is activated for every AWS customer
     - prevent `SYN/UDP Floods, Reflection attacks, layer3/4`
 - AWS sheild Advanced
     - optional DDos mitigation service
     - protection agaist more sophisticated attack on EC2, ELB, CloudFront,Route 53
 - WAF - web application firewall
     - layer 7 is HTTP vs layer 3 TCP
     - work on Application Load Balancer, APi Gate way, cloudfront
     - define web ACL (Web access Control List)
         - rule can include IP aaddress, HTTP headers
         - SQL injection and cross site scripting
# AWS Network FIrewall
 - protect ur `vpc`
 - from layer 3 to layer 7
 - u can inspect any direction
# penetration Testing
 - Aws cutomers are welcome to carry out secrity assments
# KMS & CloudHSM
 - data as rest: on hard disk, on RDS instance, in s3 ....
 - data in transit: being from transfer from premise to AWS
 - so 2 kind of encrypt, and use encryption keys
 - KMS- key management service (hear "encryption" for aws, likly is KMS
   - manages the encrytions keys for us
   - opt-in: EBS
   - 
