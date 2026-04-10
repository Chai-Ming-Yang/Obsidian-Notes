## Rule of Thumb
AWS responsible **FOR** the cloud
- "the services they provided."
User responsible **ON** the cloud
"the configurations they implemented."

E.g
User installed database on an instance of EC2:
- User responsible for the installed database's failure
- AWS responsible for the EC2 instance's failure


### AWS  *"(Security of the Cloud)"*
#### Physical Security of Data Centers
- Controlled, need-based access
#### Hardware & software infrastructure
- Compute, Storage, Database, Network
- Storage decommissioning
- Host OS  ,  Access Logging  ,  Auditing
#### Network Infrastructure
- Intrusion detection
- Region, AZ, Edge Location
- Load Balancers, Firewall
#### Virtualization Infrastructure
- Instance Isolation
#### Compliance of the Cloud
- Patches and Maintenance


## User  *"Security In the cloud"*
content stored, AWS service used, country of service
#### IAM (Identity Access Management)
- Passwords & Minimum Privilege
- **NO ROOT USER**
#### OS, Network, Firewall
- intrusion detection & prevention
#### Methodology of Storage
- Encryption  (client & server side)
- Data format  &  access permissions
- Type of content (user data / image)
- Chosen AWS Service & Country

### Oracle
- ran on EC2 instance. (user responsible)
- ran on Amazon RDS (AWS responsible)

## IaaS
- user more flexibility
- user more responsible & manage more
- user configure access control
### PaaS
- AWS manage underlying infrastructure
- AWS handle OS, database patching, firewall config, disaster recovery (DR)
- user manage implementation (code)
## SaaS
"AWS Trusted Advisor" | "AWS Shield"
- AWS centrally host software
- AWS manage underlying infrastructure
- software is licensed subscription
	- accessed through browser, API, mobile app

| DoS<br>(Denial of Service)                                            | DDoS<br>(Distributed Denial of Service)                                             |
| --------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| From same machine.<br>Same IP & Mac address.<br>Block said IP address | From different machine.<br>Different IP & Mac address<br>Hard to block individually |
 
