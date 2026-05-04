
|                 |                                                            |
| --------------- | ---------------------------------------------------------- |
| **IP Address**  | Identify device *(host & network)*<br>  - Location Sharing |
| **Port number** | Identify Endpoint                                          |
| **Subnet**      | Subdivide Network                                          |

IP Addresses
- Dynamic   |   Static
- Public    |    Private
Troubleshoot Cmd:
`ping`
`traceroute`  --> info on path taken


IPV4
- 32-bit  *(dot-separated)*
- Network Portion  *(Subnet Mask 1)*
  Host Portion *(Subnet Mask 0)*

IPV6
- Hexadecimal *(colon-separated)*
- increased security
- improved performance


Static Address
- Consistent Access
- Printers
Dynamic Address
- "changes after off/on"
- Privacy
- Mobile devices

Public
- accessible over internet
Private
- Servers *(database / application)*

|                  |                                                                                             |
| ---------------- | ------------------------------------------------------------------------------------------- |
| `10.0.0.0`       | **1st address**<br>Internet Gateway address<br>- perform NAT<br>- targeted as route address |
| `10.0.0.1`       | **2nd address**<br>Default Router Address                                                   |
| `10.0.0.2`       | **3rd address**<br>DNS Server (Domain Name System)                                          |
| `10.0.0.3`       | **4th address**<br>Reservation *(future use)*                                               |
| `10.255.255.255` | **Last address**<br>Broadcast address                                                       |

` 10.x.x.x`
`168.x.x.x`
`172.x.x.x`


 Port Numbers
combined with IP --> Determine exact src/dst of data
 - Endpoint
Can be blocked by firewall

| Port  |       |
| ----- | ----- |
| `22`  | SSH   |
| `53`  | DNS   |
| `80`  | HTTP  |
| `443` | HTTPS |




Security Group vs Firewall

| Stateful                                                   | Stateless                                                          |
| ---------------------------------------------------------- | ------------------------------------------------------------------ |
| Security Groups                                            | Network ACL *(Access Control List)*                                |
| after setting inbound rule<br>no need to set outbound rule | each packet will be checked for <br>inbound rule and outbound rule |
Inbound vs Outbound


| Security Group                      | Access Control List                                       |
| ----------------------------------- | --------------------------------------------------------- |
| Whitelist                           | Blacklist                                                 |
| Instance Level<br>(EC2)             | Subnet Level<br>                                          |
| Stateful<br>Only define allow rules | Stateless<br>Define allow & deny<br>Rule ordering matters |
|                                     |                                                           |


## Internet Gateway
- allow communication from VPC to Internet
- horizontally scaled to meet traffic needs
- highly available  &  redundant

## NAT *(Network Address Translation)*
Allow Private Subnets to access Internet
- Handled by 1st IP Address *(Internet gateway)*

## Enable internet access within console
1. Create Internet Gateway  -->  attach to VPC
2. Identify route table associated with resources
	- Add route `0.0.0.0/0`  -->  target internet gateway
3. Ensurre reource in public subnet have puvlic IP address
4. Network ACL or Security Group 


Public subnets accessible by Internet
- has IGW (Internet Gateway) routed
  accessible from outside
  
Private subnet not accessible by Internet
- NAT gateway allow internet access
  but not accessible from outside

Route Tavle
- Destination [where want to go]
- Target [where to sent it]


# Subnet
logically partitioning network

### Benefits
1. Speed 
	- reduce unnecessary traffic (ARP only subnet)
		- low congestion
	- reduce collision (>1 send data simultaneously)
		- corrupt data -> resend
2. Security
3. Conceal network complexity

| Classes                  | IPv4 size *(network id)*                                        |
| ------------------------ | --------------------------------------------------------------- |
| A `N.H.H.H`<br>`0-126`   | 8                                                               |
| B `N.N.H.H`<br>`128-191` | 16                                                              |
| C `N.N.N.H`<br>`192-223` | 24                                                              |
| D<br>`224-239`           | **Multicast**   *group comms.*<br>(No regular internet traffic) |
| E<br>`240-255`           | **Reserved**    *future/research*<br>(No public use)            |


|                    |                                              |
| ------------------ | -------------------------------------------- |
| Network ID         | uniquely identify  network                   |
| Subnet mask        | separate network & host bits                 |
| Host ID range      | host bits - 2 *(network & broadcast)*        |
| Num usable host ID | CIDR                                         |
| Broadcast ID       | target all within subnet *(last IP address)* |
"CIDR" == compact notation "Subnet Mask"
`/16`           `11111111.11111111.00000000.00000000`

CIDR allow create supernets

