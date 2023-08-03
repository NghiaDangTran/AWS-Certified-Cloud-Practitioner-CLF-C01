# Docker
 - apps are packed in containers that can be run on any os
 - docker images are tored in docker repos
 - Private docker image

![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/3c2464dc-7a7b-4357-81e3-37b7e2c4bd4a)

![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/76a2dff7-f5f9-4219-b480-7d81fd8b6008)

# ECS
 - Elastic contianer service
 - lauch Docker containers on AWS
 - you must provision and maintain the infrastruture (ec2 instacne)
 - AWS take care of start and stop container
 - has intergration with Application load balcer
 - want ro run docker container think ECS
# Fargate
 - AWS u take care the EC2
 - sverless offering
# ECR
 - Private docker repos (containe image)
 - so they can run by ecs or fargate
# Serverless
 - we just deploy code or functions
 - serverless ==Function as service
# AMZ Lambda
 - virtual functions - no server to manage
 - `short excution` after some time it will turn off
 - run on demand
 - scaling is automated
 - event driven
 - pay per call or pay per duration
# AMZ API Gateway
 - severless api
 - rest api and websocker
# Batch  
 - fully managed batch processing
 - effecient run thoundsa of computing batch jobs on aws
 - batch wull dynamically lacuh ec2 or spot instances
 - defined as Dokcer image run on ECS
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/2862d250-04c5-491b-a985-4f5f89beae57)

# AMZ Lightsail
 - virtual servers
 - simpler alternative to using eC2,eds,elb,ebs
 - greate for people with little cloud expreince
 - simple web application
 - websites
 - high availability by no auto scaling

