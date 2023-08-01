# importance
 - EBS is block
 - EFS is file system
 - object S3

# S3 - Simple Storage Service
 - Backup
 - Disater Recovery
 - Archive
 - Hybrid Cloud Storage
 - Application Hosting
# S3 Buckets
 - allow people to store object in buckets
 - `must have name unique global`
 - s3 is `match to a region`
 - They like python dict
     - key is the path to that s3://bucket/file.txt or even deep insde folder
     - `prefix +objext name`
     -  max size 5tb
     -  meta data like descrions
     -  tags - useful for security
     -  version id
# S3 Security
 - User Based: Iam Polices (only `Allow ` any `deny` will stop)
 - Resource-Based
     - Bucket Polices
     - Object Acess Control List
     - Bucket Access Controll
 - Encryption: encrypt object in S3 using encrytion keys
# S3 verioning
 - must be enable t the bucket lv
 - same key make version :1,2,3
 - easy to restore
- `importance` if u delete  specific version  it will delete that version forever
# S3 Replication (CRR and SRR) 
 - must be eable versioning
 - copy asynchonously to in region or cross region
# S3 encrytion
 - User uplaod to s3 will encrpton by AWS
 - client side encryption before upload
# Shared responsibility Model
 - Aws: Infrastructure, confirguration and culnerability analysis
 - User, versiong, bucket polices, replication
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/253f23b0-9ecc-46e4-ac7d-2ad15f210600)

# Snow Family
 - highly sercure, portable device to collect and process data at the edge
 - offline data transfer
 - if it take more than a week to transfer data use snowball
# edge computing
 - no internet access or really slow
# storage gate way
 - Aws is pushing for hybrid cloud, half on premises and half on cloud
 - just need to know this connect on server into cloud

# snowball Edge
 - physical data transport or use internet
 -  good for TBs for PBs
   -  Edge Storage (80tb hdd)
   -  Edge compute *42tb hdd ,28tb nvme
# snow Cone
 - 8tb hdd or 14tb SSD
 - use for edge computing, storage, and data transfer
 - small portable computing, anywhere, withstands harsh enviroment,can be online
 - use where snowball to big
# snowmobile
 - exabytes transfer
![image](https://github.com/NghiaDangTran/AWS-Certified-Cloud-Practitioner-CLF-C01/assets/33323750/4560eed8-8e48-45c2-8254-a4fffd12880d)

