# Elastic Load Balacing (BLB) & Auto Scailing Group (ASG)

 - `Scalability` mean the `application can handele greater loads` by adapting more server
 - there are 2 kinds of scalability:
     - `Vertical Scale` make one server stronger (t2.micro => t2.large)
     - `Horizontal Scale` add more server into the data center (=elasticity) 
 - `Scalability` is `linked but diffrent` to `high Availability`
## high availability
 - mean application in every where
 - the goal is to survive a data center loss

# Scalability vs Elasticity vs Agility
 - `Scalability`: ability to a`ccommodate a larger load` by making the `hardware stronger `(scale up), or by a`dding nodes `(scale out) 
 - `Elasticity`: once a system is scalable, elasticity means that there will be some `"auto-scaling"` so that the system can s`cale based on the load`.This is "cloud-friendly": pay-per-use, match demand, optimize costs 
 - `Agility`: fexibility and speed with which a business or individual can adapt to changes using AWS's cloud services.
# ELB ^ Elastic Load Balancing
 - are `server` that forward `incoming trafic` to mutiple ` ec2s`
 - spread load across mutiple down stream
 - seamlessly handel failures of downstream instances
 - provide `SSl` for ur website
 - high availabilty acroos zone
> aws will make sure it work, take care of upgrades, maintencae, high availability
 - can cost less to setup ur own, but more effort
# type of ELB
 - Application Load balancer (http/https only) layer 7
 - Network Load Balancer (ultra-high performace allows for tcp) layer 4
 - gateway load Balancer layer 3
![screenshot-www udemy com-2023 07 31-15_10_20](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/3eb4b725-2d42-41e2-aaef-318f244946ae)
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/1197cc85-fec7-4d61-86e8-c5bd93722b25)

# Auto Scaling Group
 -  like the name scaile ec2 based on the load of website
   -   scale out
   -   scale in
   -   ensure min and max ec2
   -   auto get new one
   -   replace unhealthy one
 - cost saving
## Scailing Srategies:
 - manual
 - Dynamic Scaling
   - Simple/Step Scailing: cliud watch check CPU % >70 add1 <30 remove 1
   - target Trancking Scailing, set an average number
   - scheduled scailingL: cron based scailing
   - predictive scailing: machine lering (good if u have predictable time based)
