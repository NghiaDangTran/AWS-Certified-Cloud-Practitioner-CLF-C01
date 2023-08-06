# AMZ CLoud Watch
 - provide metric for every service in AWS
 - metric is a stat u can monitor
     - Ec2: CPU, Status check, netowrk defalut 5 min
     - EBS volumeL disk read/write
     - s3 bucket: bucketSizeBytes, Numberof object
     - Sercvice limit
     - cutom metrix
# AMZ CLoud Watch Alarms
 - use to trigger notifications for any metric
 - alarsm actions
     - auto scailing:
     - EC2 Actions
     - SNS notification
 - billing alarm
# AMZ cloud watch logs
 - collect logs file
 - ecs,cloud trail, cloudWatch `agent` on ec2 machines and on premise servers
 - eanable real time monitoring
 - for ec2:
    - need a cloudwatch agent --> sent to cloud watch logs agent, can be on premises too
# AMZ EventBrigde
 - cron jobs, scheduled scripts
 - event pattern
# cloudTrail
 - log of all aws
 - an history of event/api calls made within ur aws
# X-ray
  - monolith easy to debug, distributed server hard to debug
  - no common views of ur architech
  - tracing of ur application, full pickture of each service
  - use for
      - troubleshooting
      - understand dependiec
      - service isus
      - throttled
      - identy users that are impacted
# CodeGruru
 - Ml service, auto code re view, application performace recomandations
     - codeGuruy reviewer: code review
     - profilers: recomand the perofrm 
 - 
