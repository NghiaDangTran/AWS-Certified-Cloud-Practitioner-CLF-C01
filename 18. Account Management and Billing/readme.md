# AWS organizations
 - global service
 - to manage `multiple AWS account`
 - cost benefits: ` aggregated usage, consolidated billing, pooling of reserved EC2 instances`
 - API is available to `automate AWS account creation`
 - `restrict account privileges using Service Control Polices`
### multi account Strategies
 - each departmeant or team should have difference isolation Service Control Polices SCP
     - Business Unit, each Business team have different account
     - Enviromental Lifcycle, divide production, develpment and test
     - Project-based -> project 1,2,3
 - AWS organiztion Units
 - like root OU  (organizations Units) -> Dev Ou or Prod Ou --> Finace Ou, HR oU 
### Service control Polices (SCP)
 - `whitelist or blacklist` IAM action
 - applied at the `OU` or `Acccounts Level`
 - `not affect Master Account`
 - `applied ` to all User and roles in the child of master account
###  AWS consolidated Billing
 - provides `combined usage` to `share` the `volume pricing, reserved instances and saving plans discounts`
 - exp: if 2 user in one org, one have 5 reserved EC2 the orther one dont have, they can share that reserved
### Control Tower
 - set up and govern a secure and compliant multi account aws enviroment
### AWS resource Access Manger (RAM)
 - share AWS resource that u own with other AWS account
### AWS service catalog
 - like a predifined catlaog that admin allow new user get and go easily
# Pricing Model
 - Pay as you go: pay for what you use
 - save when you reserve: minnize risk, oredictably mange budgets
 - pay less by using more: volume based discounts
 - pay less as AWS grow
# Savings Plans
 - Commit a certain amont per hour for 1 or  3 years
 - `Ec2 Savings Plan` commit to usage of individual  instance families in a region
 - `compute savings plan`
 - `Machine Learing plan` : sage maker
# Compute Optimzer
 - reduce costs and improve perfomance by recomending optimal AWS resource for u workloads
# Billing and costing tools
 - estimating cost in the cloud
 - tracking costs in the cloud
 - monitoring agaisnt cost plans
# Pricing calculator
 - cost calculator
# bullinfs dashboard
 - cost Allocation Tags
    - cost allocation tags to track ur AWs cost on detailed level
 - AWs genereated tags
 - User defined Tags
 - Taginf and resource groups: 
## Cost and Usage reports
 - the most comprehensive set of AWS cost and usage data available
 - can
## cost Exploer
 - visualize, understand and mage ur AWs costs and usage over time
# Billing Alarms in cloud watch
 - billing data metric for worwide AWS cost
# AWS budgets
 - send alarms when cost exedd an threshold
# AWS Anomaly detection
 - ml to detect unusual spends
# AWS service Quatas
 - notify when u are close to a service quota value threshold
# AWS trusted Advisor
 - analys ur AWS account and provides recommendataion on 5 categories
 - `cost optimization`
 - `performace`
 - `security`
 - `fault tolenrance`
 - `service limits`
 - support plans
   - 7 core chceks
     - `s3 bucket permissions`
     - sercurity group
     - IAM use
     - MFA on root accounts
     - RDS public snapshots
     - EBS public snaps shots
     - service limit
   - full check: business and enterprise support plan
     - programmatic Access using Aws support API
# support Plans
 - basic support plan
  - customer service and commnities
  - aws trusted advisor 7 cor check
  - AWS peronal Heath Dashboard
 - Developer Plan
   - business hours email access to Cloud Support Associates
   - unlimited cases/ 1 primary contact
      - case severity: general <24 hour , system impaired <12 hour
 - business support Plan
   - trusted advisor, full set of checks + api access
   - 24/7 phone email and chat access to cloud supoort engineers
     - case severity: all of the above and production system impaired <4hour, production system down <1hour
 - Enterprise on-ramp support plan
 -  all of the above, access to a pool of technial account managers
 -  concierge support team
 -  infrastruture event managemet, well architected and operations reviews
   - case severity: all of the above and business critical system down: <30 mins
- Ecterprise
- all of business upport plan, designated techinal account manger
- the smae with on rmap
   - case severity: 15 mins
