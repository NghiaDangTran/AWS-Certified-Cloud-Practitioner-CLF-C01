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
 - 
