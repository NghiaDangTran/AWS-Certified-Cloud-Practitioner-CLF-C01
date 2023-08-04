![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/1e7b671f-ada4-42d3-81df-e12a9d303dc4)
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/34beb739-9312-4b2f-9698-39c1ac85e6d4)


# Cloud Formation
 - is a declarative way of outlining ur AWS
 - exp:
     - u want a security group
     - ec2 using that security group
     - a s3
     - load balncer in front of these
  - could formaton creates thoose for u, in the right order, with the exact confirguaraion that u specify ( auto do)
  - infrastruture as code
      - no resuorce are manually created
      - change to the infra are do as code
  - cost: they stack in tagged groupo so easier to identy fy cost
  - Productivity
      - ability to destroy and recreate infra on the cloud on the fly easy
      - automated generation of diagram
      - declarative programing
  - Dont re invent the wheel
 - use infratreuc as code, or need to rebuld the infra easily on anywhere
# AWS BeanStalk
 ## Dev problems on AWS
  - managing infrastructure
  - deploying code
  - configure data base, load balncer
  - scailing
 then beanStalk will take care all of that developer centric
 - beanstalk =platform as service (only care code)
 - managed sercive, handel by aws
 - three architecuteL
     - single instance. developemt env
     - lb and asg good for production or pre production
     - ASG, good for non web apps
# AWS CodeDeploy
 - work ` hybrid` both on ec2 and on premises
 - must have codepley agent or server
# AWS Code Commit
 - store code
# AWS code build
 - complie source code, run test, produce pre compile package
# AWS CodePipeline
 -- orchestra the diffrenct steps to have to code auto matically push to productipn
 - auto push to production
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/d98b5d33-e014-4ddc-9f7d-3e7417d5afd9)
# AWS codeArtifact
 - like the node_modelue where u can call to code build or urself
 - like build npm then public it and sise
# Code Star
 - one stop
 - with ui quick way to get start
# cloud9
 - online IDE can share with mutiple preople
# System Manger (SSM)
 - manage EC2 and Premise system at s cale
 - hybrid aws
   - patching automation for enhanced compliance
   - run commands across an entire fleet
   - store parameter:
   - key run command acroos server
 - Session Manager need port 22 to acess
# AWS OPSWorks
 - chef and pupet help u perform server configuration automatically or repetitive actions
 - work great with ec2 and on premies
 - chef or pupet >>> ops work
 - 
