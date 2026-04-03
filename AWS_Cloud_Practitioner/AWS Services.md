https://docs.aws.amazon.com/
https://docs.aws.amazon.com/pdfs/whitepapers/latest/aws-overview/aws-overview.pdf

![[aws_services.png]]
![[aws_services2.png]]
![[aws_services3.png]]
# Storage
#### S3 (Simple Storage Service)
Slower access
- **S3 Bucket** - Instant public access (GDrive)
- **S3 Glacier** - Slow access (backup) (infrequent Access)
#### EBS (Elastic Block Store)
- private access file
#### EFS (Elastic File System)
- Linux Only (X window)
- shared file

# Compute
#### EC2 (Elastic Computing Cloud)
- **EC2** - 
- **EC2 Auto Scaling** - 
- **EC2 Reserved Instance** - long term commitment discount (subscription)
  Upfront Cost : No / Partial / Full
#### Elastic Beanstalk 
- Complete Application
#### Lambda
- Function (event driven) **PaaS**


# Container
"must be installed for EC2 instance"
#### ECS
- 
#### ECR
#### EKS
#### Fargate
- manage underlying infrastructure
- ECS, ECR, EKS require manual infrastructure management

# Database
#### RDS (Relational Database Service)
- RDBMS fixed schema
#### Aurora
- RDS database by Amazon (more costly)
#### Redshift
- Big Data (Terabytes)
#### DynamoDB
- Unstructured data (MongoDB)
#### DocumentDB
- MongoDB compatible (just paste)

# Networking / Content Delivery
#### VPC (Virtual) ⭐
- Create subnets
#### Elastic Load balancing
- multiple EC2 instances doing same thing
- Application & Network & Gateway
#### CloudFront
- Cache 
#### Transit Gateway
- Connect >1 VPC together (Star schema)
#### Amazon Route 53
- Redirect (Proximity, Geographical, )
#### Direct Connect
- Direct connect with on-premise Data Center
#### Client VPN
- 

# Security, Identity & Compliance
#### Identity & Access Management
Role Defining : Developer / Testers / Managers
#### Organizations
- multiple companies to handle
#### Coginto
- Authentication
#### Artifact
- 
#### Key Management Service
- Encryption
#### Shield
- DDoS Protection




# Cost Management Services
#### AWS Cost & User Report
- exceed % of budget, email notification
#### AWS Budget


# Managemenet & Governance Services
#### Management Console
#### Config
#### CloudWatch
#### Auto Scaling
#### 
#### 
#### 
#### 

