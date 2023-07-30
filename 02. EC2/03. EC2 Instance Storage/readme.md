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
