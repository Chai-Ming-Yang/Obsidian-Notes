**Asset Inventorying**
- Devices
- Servers
- Applications

## AWS System Manager
|                          |                                                             |
| ------------------------ | ----------------------------------------------------------- |
| Installed Applications   | Name, Version, Publisher<br><br>                            |
| Installed AWS Components | EC2, Drivers, Agents (File System Manager agent)<br><br>    |
| Network Configurations   | IP & MAC Address, Subnet Mask, DNS<br>Exposed Ports<br><br> |
| Windows Updates          | Hotflix ID, Installed by, Install date<br><br>              |
| Files                    | Name, Size, Version, Date (Create/Modify/Access)<br><br>    |
| Services                 | Name, Status, Dependency, Type, Autostart                   |
| Instance Details         | Name, OS (version / architecture)                           |


**CVE *(Common Vulnerabilities & Exposure)***


# Assessments
|                 |                                  |
| --------------- | -------------------------------- |
| **Host**        | evaluate server vulnerability    |
| **Network**     | evaluate network accessiblity    |
| **Data**        | examine protection level (CIA)   |
| **Application** | evaluate security of source code |

# Countermeasure
|                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Network Hardening                | **discovery hardening**<br>*"prevent discover, explore, mapping network"*<br>- block network exploration protocols<br>- block unused ports<br>- up-to-date inventorying<br>- limit remote administration access<br>- security groups (instance level)<br><br>**security architecture**<br>- Firewalls  &  IPS *(Intrusion Prevention System)*<br>- Segment Network<br><br>`ping` test host reachability *(online)*<br>`traceroute` intermediate devices<br>`nmap` scan open ports<br>**traffic sniffing**<br>- read unencrypted session data *(password)*<br><br>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| System Hardening<br>(host level) | *"Least functionality"*<br>- OS security updates<br>- Remove unused app/service<br>- Monitor & Control configs<br><br>*Establish Baselines*<br>- policies   &   rules   &   audit<br>- consistency  ,  prevent misconfig<br><br>Authentication Authorization Accounting<br><br>Harden <br>= Server : min exposed services<br>= Application : update dependencies<br>                         restrict permissions<br>= Cloud : secure IAM permission<br>                encrypt storage<br><br>Training & Education *--social engineering*<br> - stop someone without badge<br> <br>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Data Security Controls           | Protect Data from<br>  *unauthorized access/modify/disclose/destruct*<br>- Encrypt   *(Confidentiality)*<br>- Hash       *(Integrity)*<br>- Backup    *(Accessibility)*<br>- Digital certificates<br>- Data integrity checking tools<br><br>- RBAC   *Role-Based Access Control*<br>   = centralized<br>   = scalable  ,  inheritable  ,  least privilege<br>- DAC     *Discretionary Access Control*<br>   = decentralized<br>   = permission may spread uncontrollably<br>   <br>Encryption  - *reversible*<br>- Symmetric    ==AES==<br>   (fast) (bulk)<br>- Asymmetric  ==RSA==<br>   (public private key pair) (scalable management)<br>   (Non-repudiation)   *3rd-party unable deny involvement*<br><br>Hashing  - *one-way*<br><br>Data States <br>- at rest        *(Drive Encrypt)*<br>- in transit    *(SSL / TLS)*   <br>                     *(Kerveros)*  {2 device comms.}<br>					 *(IPsec)*        {foundation of VPN}<br>- in use        *()*<br><br><br>**Certificate Authorities**<br>- issue certificates, manage trust relationships.<br>- internal (free) (trusted within organization)<br>- Extermal (paid) (trusted by every entity)<br>==CPA== Certificate Practices Statement <br>- stamdards / algorithms <br>Root CA<br><br>**Revocation Lists**<br>- Expiration and Revocation <br>- ==OCSP== *(Onlinr Certificate Status protocol)* |
| Identity Management              | Active Administration of Access Permissions<br>"Scalable"<br><br>- Least Privilege<br>- Set & Enforce Policy<br>- Principles of AAA<br>==Identification== prove identity<br>==Authentication== validate identity<br>==Authorization== determine permissions<br>==Accounting== establish audit measures, log access history<br><br>Passworkd Policies<br>- MFA, Aged password. complex<br><br>Attacks:<br>- Rainbow Table    (precomputed hashtable)<br>- Dictionary           (real-time hashing attempts)<br><br>Tools<br>- Password Managers<br>- SSO *(Singe Sign-on)*  {sign-in with google}<br>- Federated User <br><br>"Something you ..." {know , have , are}<br><br>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

## Layered Security Model
|                          |                                                         |
| ------------------------ | ------------------------------------------------------- |
| **Perimeter Security**   | Firewall<br>IPS *(Intrusion Prevention System)*<br><br> |
| **Network Security**     | NACL *(Network Access Control List)*<br><br>            |
| **Endpoint Security**    | Antivirus (protect host)<br><br>                        |
| **Application Security** | Monitoring & Scanning Tools<br><br>                     |
| **Data Security**        | IAM *(Identity Access Management)*<br><br>              |


**AWS - FLEET MANAGER**

**Amazon Inspector**
- identify open ports / exposed EC2 instance


**AWS Trusted Advisor** 
- recommendations of best practices
**Amazon GuardDuty**
- Threat *(malicious IP)* detect, continuous activity monitoring
**AWS Shield**
- DDoS protect
**AWS CloudTrail**
- record + monitor API activity or user actions
- {action} {time} {location} {by who} {response}
- simplified compliance
- analysis + troubleshoot
- always-on
- "Aggregate log files into S3"   *.gz extension*
  "Integrate Amazon CloudWatch"

**Amazon CloudWatch**
- monitor cloud resources + applications
- health / performance / alarms

**AWS Config**
create rules , **alert** upon violation
- assess configs (compliances , changes) of AWS resources 
- "Implement with AWS CloudTrail"

**AWS CloudHSM** Hardware Security module
- Dedicated Hardware
- exclusive ownership *(single tenant)*
- high compliance environment
**AWS KMS** Key Mgmt Service
- Software-Centric
- create / rotate / delete   keys
**Amazon Certificate Management**
- SSL/TLS Certificates  {provision, manage, deploy)

**AWS SSO** Single Sign-On
- one-click access aws account
- common cloud app compatible
**Amazon Cognito**
- for web & mobile app
  manage, authenticate, authorize users
**AWS IAM** Identity Access Management
- create, manage {group / role *(temporary access)*}
- password-less permission granting
- AWS Service Integration
- Identity Federation
- ==trust== -- specify entity
- ==access== -- specify accessible action/resource
Explicit Deny/Allow   +   Implicit Deny
- Policies {standalone} - reused      {inline} - 1-to-1

