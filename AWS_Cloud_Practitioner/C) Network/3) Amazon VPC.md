| Traditional Topology                                           | AWS Services                                                                                 |
| -------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| **Data Centers**<br>- setup & maintain<br>- need >1 components | **Amazon VPC**<br>- no maintenance required                                                  |
| **Router**<br>- Filter packet<br>- Route traffic               | **Route tables**<br>- input route within VPC                                                 |
| **Switch *(Subnet)***<br>                                      | **Subnet**<br>- logically isolate IP groups                                                  |
| **Firewall**<br>- *Node level* traffic blocking                | **Security group<br>Network ACL *(Access Control List)***<br>- Subnet Level traffic blocking |
| **Server & OS**                                                | **Amazon EC2**                                                                               |
| **Modem**<br>- internet from ISP                               | **Internet gateway**                                                                         |
- Select IP address range
- create subnets
- config routing table
- security features


## Features
1. Dedicated AWS Account
	- to access AWS Cloud
2. Belong to single AWS Region
	-  >1 AZ *(Availability Zones)*
3. Logically isolated from other VPC



IP Address in Amazon VPC
- specify IPV4 *(choose CIDR block)*
	- Classless Inter-Domain Routing
	- `10.0.0.0/16`   "the `/16` is CIDR notation"
Recommend: Avoid using CIDR block outside of private range
- may cause issues



