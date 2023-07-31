# EBS
 - An EBS (Elastic Block Store) `Vloume` is a `Network` drive you can attach to your instances while they runing
 - it `allows` yor instances `to presist data` even after theier termination
 - `only one instance at a time`
 - `vound to a specific availability zone`
> think like `"network USB stick"`
# EBS Volume
 - it's a `network drive`
     - it use the netowrk to communicate the instance, might have a bit latency
     - it can de detached from an EC2 instance and attached to another one quickly
 - `lock to an Availability Zone `(AZ), but can use `snap shot` to move around
 - have `many type of capacity `like size, IOPS
     - `billed` for all the` provisioned capacity`
     - you can `inscrease the capcity over time`
# EBS Snáphót
 - make a backup of EBS
 - dont need to detach EBS but recommended
 - can copy snapshots across AZ
![screenshot-www udemy com-2023 07 30-15_10_37](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/433735e3-b6e1-4c23-b8f9-f95896d846a9)

 - EBS snapshot archive -> 75% cheaper, take 24-72 to restoring 
 - Recycle Bin for EBS, can recover deleted EBS (set from 1 day to 1year)


# AMI
 - Amazon Machine Image
 - AMI are a `customization of` an `EC2` Instance
    - add own software, configuration,...
    - faster boot/ configuration time
 - build for `a specific region` , can copy across regions
 - can lanuch EC2 instance by:
    - A public AMI
    - your own AMI
    - AWS marketplace AMI
  
 ## process
  - start an ec2 and customize
  - stop it
  - build AMI from the ec2 snapshots
  - lauch new EC2 from that snap shots
# EC2 Image Builder
 - Used to automate the creation of virtual machines or container images
 - => automate the creatio, maitain, validata and test `EC2 AMIs`
 - this AMI can be distributed mutiple regions
 - can run on a schdule, and also can be tested
 - free (only pay for the underlying resource)
 - Helps ensure your applications run on a stable, secure, and up-to-date platform.
# Ec2 instance Store
 - EBs is good but `Instance Store is higher peroformance`
 - better I/O performance
 - but not like EBS one `stop it lose data`
 - good for buffer /cached/scratch data
 - risk of data loss if hardware fail
 - must backup
 - trick `really high IOPS mean inctance store
# EFS elastic File System
 - Managed NFS(network file system) that can be mounted on 100s EC2
 - work with Linux only and have multi AZ
 - high available, scalable, expensi ve, pay per use

![screenshot-www udemy com-2023 07 30-20_34_33](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/fb86d5c2-78cd-4ced-a7ec-50139f20a73c)

## EBS vs EFS
 - EBS use the snapshot (copy) to share btw EC2
 - EFS share directly with all the EC2

# question what is the diffrent btw AMI and Image builder
