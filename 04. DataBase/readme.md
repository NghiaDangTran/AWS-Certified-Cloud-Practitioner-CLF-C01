# DataBase
While EFS, EBS, EC2 is really good, but sometime you may want somethingmore struture, to build index to effcient query/ serach
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/717b8eaa-5dc3-4d81-97a8-ce121da31554)


# Relational Databases
 - llooks like excel but links btw them
 - can use SQL languae to perform queries
# NoSQL Database
 - are built for specifc data models and have flexible schemas for building mordern application
     - flexibility
     - scalability
     - high-performance: optimiezed for a specific data model
     - high functional: type optimized
     - JSON

# Databasese and Shared Responsibility on AWS
- AWS offer to usr to manage diffrent database
    - quick provisioning
- techinaly u can host everything on ec2, but u must handel everything urself, even incase of diadster, also AWS DB u cant ssh into ur instaces

# AWS RDS (Relational Database Service)
 - is Aws Databse for SQL language
 - postgres, mySQL, oracle...
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/82ed5346-44ad-4cc4-9460-7fd67d32deeb)
# AWS Aurora
 -  is a property technoly from AWs( not open source)
 -  they do support ` postgreSQL and MYSQL`
 -  they said it is `AWS cloud optimized` which they say 5x better than postgreq SQL
 -  and the cool thing is ato scale size, from 10GB up to 128TB
 -  20% expenssier but is more effcient too
 -  also u can take snapshot too,
# RDS Deployments
both write operation is directly to the main db, ortherwise it read directly
 - read Replicas:
   - scale the `read` workload of yout Db
   - upto 15 read replicas
   - good for, recovery, run db report, read distribution
 - Multi-AZ
   - set up more clone DB in orther AZ
   - loss prevention
 - multi-region
  - set in more region
  - better local performace
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/4eea98fe-b0c0-47be-86c8-56cbed0fb795)
# AWS ELastiCache
 - is to get managed Redis or memcached
 - `in-memory db` high perfomace low latency
 - `reduce load off dabased for read intesive workload`
 - AWS take care of OS, backup
 - can use with anyhting
# AWS Dynamo DB
 - is NoSQL databse, can replication across 3AZ
 - scales to massive workload, distributed `serverless` database
 - `low latency retrival`
 - keyword: serveless, sub milisconds latency
 - remmber u only table, no need to create database
## DynamoDB Accelerator -DAX
 - inmemoery cached for dynmodb
 - 10X performance
 - only use with Dynamo DB
## DynamoDB lobal Tbales
 - low latency, mutiple regions
 - active-active replication, read write update to any aws region
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/20a23f36-32ca-426f-a9f4-4d1ac0890d20)

# Readshift (analytical processng)
 - basedon PostgreasSQL but not OLTp (on live transaction processing)
 - but it is OLAp (online analytical processing)
 - load data slow
 - `coloumnar` strorage
 - 10x better performace
 - use massively Parallel query execution
# Amz EMR
 - hadoop cluster (big data)
 - made of cluster of server
 - data processing, machinge learning, web indexing
# AMz athena
 - serverless query serive, peform analytics againse s3 object
 - use sql to query s3
 - fllow `athena query data ==> quick shight report`
 - s3, sql=> athena
# AMZ quícight=> make report
# DocumentDB
 - is the mongoDB, auto scale
 - DynamoDB scales by adjusting read and write capacity, while DocumentDB scales by adding more instances.
# Neptune
 - Graph Daabase
# QLDB
 - Quantum Ledger Databse
 - `recording finanacial transactions`
 - erview history of all the changes made to ur data
 - immutable
 - no decentralization component
# Managed Blcockchain
 - join public blockchain
 - decentralization compoonet
# Glue
 - extract, transform and load
 - serveless service
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/9478c6ce-29de-439a-9c38-94c073fbd4f9)
# DMS
 - database migration service
 - database migrate from source db to aws 
