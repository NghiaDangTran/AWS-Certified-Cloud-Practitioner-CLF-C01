# EC2 Setup

`instance` refers to a `virtual server` in Amazon's Elastic Compute Cloud (EC2) for running applications on the Amazon Web Services (AWS) infrastructure. 
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
 # Never do `AWS configure` it will save on that Ec2 and they can retreive it (do by IAM)
# Purchasing Options
 - On-Deman instances: short workload, predictable, pay by second
 - reserved ( 1-3 years)
    - reserved instances - long workloads
    - convertible Resvered instances - ling workloads with flexible instances
 - saving plans (1.3 yeas) : commitnet to an amount of usage, long workload
 - spot instace: short work load cheacp, can lose instance (less reliable)
 - dedicated hoost: book an entire physical servcl, control instace placement
 - dedicated instance: no orther people will share your hardware
 - capacity reservation: reserve capcity in a specific AZ for any durtion

## On Demand: (good for `short and uninterupted` where u `cannt predict` what u need)
 - linux and windows billing by second
 - all orther image billing per hour
 - highest cost, but no upfront payment, no long term comitend
 - good for `short and uninterupted` where u `cannt predict` what u need
## Reserved Instances: allways on usage applications
 - up to 72% save
 - reserve a specifc instance attribute (instance Type, region enancy,os)
 - Reservation Period — I year (+discount) or 3 years (+++discount)
 - Payment Options — No Upfront (+), Partial Upfront (++), All Upfront (+++) 
 - Reserved Instance's Scope — Regional or Zonal (reserve capacity in an AZ)
 - Recommended for steady-state usage applications (think database) 
 - You can buy and sell in the Reserved Instance Marketplace
     - convtible Reserved instance
     - can cahnge the ec2 intace type, family, os, cope tenacy
     - up to 66% sale
## Saving Plans (good if u know what u may need)
 - discount based on long term
 - commit to certain type of usage `10/hours for 1 or 3 years`
 - Usage beyond that commit go to On-demand
 - locked to a specid instace family and AWS region
 - flexible across:
      - instace size
      - OS
      - tenancy
## Spot instances: if u know u can pause the work
 - max discount, but can lose
 - the most cost-efficent
 - Batch jobs
 - data analysis
 - image processing
 - andy `distributed workload`
 - with a flexible start and end time
 - not for creitcal jobs or databse
## dedicated Host (control entire of hardware, no one can use it, u can controll the hardware) 
 - a physical server with ec2 instace capacity fully dedicated to ur use
 - Save money on licensing costs
 - compliance requirement 
 - purchase : on deman and reserved, the most expensive one
 - use for software that have complicated licensing model (breing your own license)
## dedicated instances (instance is u only, but not hardware, u cant control hardware)
 - run on harware that dedicated for u
 - may share haredware with other in same accnot
 - This means that Dedicated Instances may share the same underlying hardware with other instances from the same AWS account that are not Dedicated Instances.
## capacity reservations: `short term` uninterupted workload 
  - reserve on deman instances capacity in a specifc AZ for any duration
  - no time commnet , no bill discounts
  - for `short term` uninterupted workload that need to be in a specifc AZ

![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/fdded8e2-aaf8-43c4-8a27-157a354f7da6)
