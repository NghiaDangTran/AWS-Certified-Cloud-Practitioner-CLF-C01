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
