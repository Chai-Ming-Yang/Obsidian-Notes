#### Compute Services
1. VM
2. Container
3. PaaS
4. Serverless

| AWS EC2                            | Amazon Lightsail                                                     |
| ---------------------------------- | -------------------------------------------------------------------- |
| manual setup                       | all-in-one, preconfigured interface<br>(server, storage, networking) |
| Variable Price (pay as you go)     | predictable pricing (fixed)                                          |
| Granular control over CPU & Memory | Less customization & scalability                                     |
##### AWS Outposts
- Run AWS infrastructure and services on premise
##### AWS Batch
- Run batch job at any scale


EC2 Server:
App, Web, Database, Game, Mail, Media, Catalog, File server, Computing server, Proxy

## EC2
Full control over **Guest OS**
Launch instance any (size & AZ's)
- from AMI (Amazon Machine Image)
## (9) Decisions in AWS Management Console
### 1. AMI
specified source of **AMI** to run an instance
e.g. (Quick Start)  ,  (My AMI)  ,  (Marketplace)  ,  (Community)
#### Benefit
**Reusability**: Multiple instances of EC2 from same AMI
**Repeatability**: 
**Recoverability**: Restorable backup from configured instance.
### 2. Instance Type
- RAM, CPU, Storage, Network
Instance Type Categories
- General Purpose  &  Compute Optimized  &  Accelerated Computing
  Memory Optimized  &  Storage Optimized
Naming: t3.large
- T (family name)
- 3 (generation)
- Large (size)
### 3. Network Setting
### 4. IAM role
### 5. User data
### 6. Storage options
**EC2 Instance Store**: 
- Fast access (RAM)
- Ephemeral (tmp) storage
Amazon EBS
- Persistent Storage
### 7. Tags
### 8. Security Group
### 9. Key pair
a pair of "public key" & "private key"
connect to EC2 instance form Powershell


aws ec2 run-instances \ 


## Pricing Models
| Instance           |                                                                                                                                                                                                                                                                                        |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| On Demand          | Pay by the hour<br>No long term commitments<br>Eligible for **AWS Free Tier**<br>"Spiky unpredictable traffic"                                                                                                                                                                         |
| Reserved           | Full/Partial/No upfront payment<br>1-year or 3-year term<br>Discount on hourly charge<br>                                                                                                                                                                                              |
| Spot               | Ran when available when user's bid > market price<br>Can be interrupted by AWS<br>    - 2-minute notification<br>    - post interruption (terminate / stop / hibernate)<br>Significantly **less expensive** than **On-Demand**<br>"for application with flexibility in running timing" |
| Dedicated Hosts    | Physical server with EC2 instance capacity<br>    - fully dedicated                                                                                                                                                                                                                    |
| Scheduled Reserved | 1-year term<br>capacity reservation for specified                                                                                                                                                                                                                                      |
| Dedicated          | Run in a BPC on hardware<br>    - dedicated to a single customer                                                                                                                                                                                                                       |
| Per-second billing | available for <br>    - Spot Instances<br>	- On-Demand Instance<br>    - Reserved Instance                                                                                                                                                                                             |
Reboot preserve data on Amazon EC2
- since reboot needs OS 
Security Group is whitelist not blacklist
- allow all outbound traffic by default
- 
