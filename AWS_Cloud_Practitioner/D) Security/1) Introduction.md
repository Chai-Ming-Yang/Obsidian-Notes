# Cybersecurity 
- protect network / device / system, digital information
	- Unauthorized Access
	- Malicious Modification, Theft, Destruction
	- Disruption of intended use

## CIA 
|                     |                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------- |
| **Confidentiality** | Prevent unauthorized access (protected)<br><br>==Authentication==<br><br>                                |
| **Integrity**       | Authentic original (untampered) data<br><br><br><br>                                                     |
| **Availability**    | Accessible when needed<br><br>BCP *(Business Continuity Plan)*<br>DRP *(Disaster Recovery Plan)*<br><br> |

## Cost of Data Breach
- Damage business reputation
- Lose customers
- Lose resources / data
- Stolen Identity
- Resolve breach takes time

# Threats
|                            |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | CIA                                          |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| Malware                    | Malicious software<br>- disrupt operation of system<br>- gain unauthorized access<br>- collect sensitive data<br><br>Virus -- corrupt/delete data<br>         -- self-propagate<br>		 -- spread on user action <br>Spyware -- gather info (key logger)<br>Worm -- Automatic execution<br>           -- Spread to all host <br>		        - on same network<br>		   -- Consume Network Resource<br>		   -- Slow Performance<br>		   -- Install Backdoor<br><br>RAT *(Remote Access Trojan)*<br>           -- gain unauthorized access | Confidentiality<br>Integrity<br>Availability |
| RansomWare                 | Malicious code<br>- restrict access until ransom paid<br><br>                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Availability                                 |
| DoS *(Denial of Service)*  | Prevent access<br>- of authorized user<br><br>DDoS -- Exhaust reource<br>          -- multiple device different region<br><br>                                                                                                                                                                                                                                                                                                                                                                                                      | Availability                                 |
| MitM *(Man-in-the-Middle)* | Intercept communication<br> - Impersonate <br> - Modify communication<br><br><br>                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Confidentiality<br>Integrity                 |
| Phishing                   | Fake masquerades as legitimate<br> - get personal info (credit card, etc.)<br><br>                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Confidentiality                              |
| Social Engineering         | Manipulation<br><br>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Confidentiality                              |

# Security Strategy
- WHAT + WHEN + WHO
- prevent threats  |  eliminate vulnerability  |  recover from breach

|                             |                                        |
| --------------------------- | -------------------------------------- |
| **Security Control**        | **`WHAT`** security measures implement |
| **Security Lifecycle**      | **`WHEN`** to implement                |
| **Security Responsibility** | **`WHO`** responsible to implement     |

| Security & Responsibility                            |                                                                                                                                                                                                            |
| ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **IN** the cloud<br><br>Customer Responsible<br><br> | - customer data<br>- applications & IAM<br>- OS, network/firewall config<br>- data encryption (client/server-side)<br>- data integrity authentication<br>- network traffic protection<br><br>              |
| **OF** the cloud<br><br>AWS Responsible<br>          | - AWS Services<br>    { Compute, Storage, Database, Networking }<br><br>- AWS Global Infrastructure<br>    { Region , Availability Zones }<br>    Data Centers<br>	"Virtualization of Maintenance"<br><br> |

# Security Controls
|                | Physical<br>*(Hardware)* | Administrative<br>*(Policy / Procedure)*                      | Technical<br>*(Software)*                        |
| -------------- | ------------------------ | ------------------------------------------------------------- | ------------------------------------------------ |
| **Preventive** | *Card Reader*            | *swipe card to access*                                        | *collect card data*<br>*monitor building access* |
| **Detective**  | *Metal Detector*         | *Mandate reports per <br>  system change*                     | *Antivirus routine scan*                         |
| **Corrective** | *Backup Generator*       | **BCP** *(Business Continuity Plan)*<br> - critical functions | *Antivirus <br> auto remove malware *            |

# Security LifeCycle
|                   |                                                                                      |
| ----------------- | ------------------------------------------------------------------------------------ |
| **1) Prevention** | - Identify assets<br>- Assess vulnerabilities<br>- Implement countermeasures<br><br> |
| **2) Detection**  | - Monitor & Detect security issues<br>                                               |
| **3) Response**   | - Respond to issue<br>- Restore operations<br><br>                                   |
| **4) Analysis**   | - Analyze issues<br>- Update policies & procedures<br><br>                           |

