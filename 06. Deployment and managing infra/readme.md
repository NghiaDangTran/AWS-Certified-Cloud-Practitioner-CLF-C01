# Cloud Formation
 - is a declarative way of outlining ur AWS
 - exp:
     - u want a security group
     - ec2 using that security group
     - a s3
     - load balncer in front of these
  - could formaton creates thoose for u, in the right order, with the exact confirguaraion that u specify ( au to do)
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
