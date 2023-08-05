![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/e7ddb427-bcd4-42c3-94fa-a6d0bd53aa4a)

# introduction
 - we need to comnicate btw mutiple application
     - Synchronous comnucations, (connect appplications to applications)
         - cannot handel spikes of traffic, may fail
     - Ayschorous ( middle ma, queue in btw)
  
# AMZ SQS
 - compose of producer --> queue --> consumer
 - oldest AWS server
 - serveless, use to decouple applications
 - scale 1 mess/sec to 10000/mess/sec
 - message are deleted after they're read by
# AMZ Kinesis
 - real time big data streaming at all scale
 - managed service to collect, porcess and analyze rtealt time streaming data
# AMZ SNS
 - email, phone notifications
 - oone publiser but can send mutiple sucrebiber
# AMZ MQ
 - managed message broker service for rabbitMQ, active MQ, doenst scale as sqs, sns
 - run on server, can run multi AZ with failer
 - 
