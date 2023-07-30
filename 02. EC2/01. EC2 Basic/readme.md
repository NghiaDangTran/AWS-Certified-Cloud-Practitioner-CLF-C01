# EC2
 - one of the most famous service
 - Infrastruture as a service 
 - consist of:
   - renting virtual machine (ec2)
   - storing data on virtual drives (EBS)
   - Distributing load across machine (ELB)
   - Scaling the service using an auto-scaling group (ASG)
- `fundemental` of how `cloud work`
# Sizing & Configuration
 - operating system
 - CPU
 - RAM
 - Stroage need
     - network attached (EBS and EFS)
     - hardware (EC2 instance store)
  - netword card
  - firewall rule: `security group`
  - Boóttrap script: EC2 User Data
# EC2 User Data
 - make it run some thing until we login (boostrap)
 - `boostraping` mean launch  command when a `mahcine start`
 - can be use to do:
    - install update
    - software
    - download common files
    - anything else
 - run with root user (sudo command)
# Ec2 instance Type:
 example: `m5.2xlarge`
  - `m` stand for class of the cpu
  - `5` generation of AWS
  - `2xlarge`: size with the instance class(how strong)
 ### general purpose
 - balance btw compute
 - memory
 - networking 
 ### Compute Optimized
  - batch processing workload
  - media transcoding
  - high performance web servers
  - high performace computing(HPC)
  - scientific modeling and machine learing 
  - gaming servers
 ### Memory Optimized  (RAM)
  - hight performace relation/ non relational database (Redis or memcahce)
  - distributed web scale cache stores
  - in memory database optimzer for BI
 ### Storage Optimied (High IOPS)
  - high ssd or hdd
  - database
