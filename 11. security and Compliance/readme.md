![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/942b874e-ebc2-4107-aa4c-af8610691725)
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/b3f4d674-c057-4206-9845-0422d2fd74d8)

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
   - opt-in: EBS ,s3 ,redshift, data warehouse
   - automatically encryption: cloudTrail Logs, S3, Stroage Gateway
 - AWS manages the software
# cloudHSm
 - HSM -phusicall server just for generate and store secret key
 - AWS manages the hardware
 - Type of CMK  customer master key
    - customer Managed CMK: user create manage and used by the customer, can eable or disable
    - AWS managed CMK: created, managed and use on the customer behalf, use by AWS service
    - AWS owned CMK: KMS service, application only
    - cloudHSM keys: AWS lend hardware to u
# ACM certificate Manager
 - SSl/TLS certiface
# AWS secrets Manger
 - newer service, mean for storing secrets (like ENV)
 - totation secret every X days
 - secrets are encrytped using KMS
# AWS artifact (not a service)
 - provide customers with on demand access to AWS compliance document  and AWS agreements
# AMZ GuardDuty
 - ML threat discovery to protect AWS account
  - check could trail events logs
  - VPC flows logs
  - can protect against crytoCurrency attack
# AMZ inspector
 - automated security Assessments
 -  for EC2
 -  for continaer images push to AMZ ECR ( container regfister)
 -  lambda functions
# ANZ config
 - help s with auditing and recording compliance of ur AWS resources
 - record configurations and changes over time
 - mainly just to check critcal compliance
# AMZ Macie
 - ML and patterm matching to discover and protect ur sensitive data in AWS
 - detect sensitive data
# AWS security Hub
 - central security tools, manage across several AWS accounts and automate security checks
# AMZ Detective
 - deeper analysis to isolate the root case and take action of security issue, ML and gprahs
# AWS Abuse
 - suspected AWS resources used for abusive or illegal purpos
 - Spam, Port Scanning, Dos, DDos, instrusion attempts, hosting
# Root User Preivileges
 - Never use Root
 - **chane account settings (account anme, email, user ,)**
 - tax invoices
 - **close AWs**
 - restore IAm
 - **change or cancel AWS supprot plan**
 - **register a seller in reserved**
 - configure S3 bucket to eabnle MFa
# IAM access Analyzer
 - findout which reoruces are shared externally
 - **defind Zone of Trust** = AWS acocnt or AWS org
 - recomend what should be the IAM for them
