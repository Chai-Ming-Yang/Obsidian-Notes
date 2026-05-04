
|                                      |                                           |
| ------------------------------------ | ----------------------------------------- |
| WEP <br>*(Wired Equivalent Privacy)* | encrypt data, secure wireless network     |
| WPA<br>*(Wi-Fi Protected Access)*    | security keys & user auth.<br>replace WEP |
| BLE<br>*(Bluetooth Low Energy)*      | energy efficient<br>IoT                   |
| 5G Cellular system                   | 10Gbps                                    |

# IoT
physical device -- connected to internet -- share & collect data
"smart device" --> Device Gateway --> IoT Platform --> UI

|                                             |                                                                                                  |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| MQTT<br>*(MQ Telemetry Transport)*          | lightweight , publish-subscribe<br>low-bandwidth , high-latency , unreliable<br><br>             |
| HTTPS<br>Hypertext Transfer Protocol Secure | upload data to cloud<br><br><br>                                                                 |
| WSS<br>Web Socket Secure                    |                                                                                                  |
| BLE<br>*(Bluetooth Low Energy)*             |                                                                                                  |
| LoRaWAN<br>Long-Range Wide Area Network     |                                                                                                  |
| Proprietary RF (radio frequency)            |                                                                                                  |
| POP (Post Office Protocol)                  | Email (Layer7)<br>retrieve msg from remote mail server to local device<br>msg deleted afterwards |

### Enterprise Mobility
- remote-work option
- **BYOD** *(Bring Your Own Device)*
- **MDM** *(Mobile Device Management)*
  enforce policy

# Amazon WorkSpace
- Virtual Cloud-based Desktop *(Microsoft / Linux)*
Authentication : (AWS Directory Service)  (Microsoft Active Directory)
### Simple Mgmt
Amazon WAM *(WorkSpace Application Manager)* 
- Deploy & Manage applications
### Secure
- Authentication
AWS Directory Service  /  AWS Managed Microsoft Active Directory
### Scale **Up** consistently
- size of root user  &  user volume per WorkSpace
- 1 expansion allowed per 6 hour
- **to scale down** --> create new WorkSpace --> Migrate
	*(Data Integrity)*



Secure web app
- SSL *(Secure Sockets Layer)*
- TLS *(Transport Layer Security)*

Proprietary Microsoft Protocol
-  RDP *(Remote Desktop Protocol)*

`tcpdump`
- list network traffic *(real-time)*
	- passing through network interact
`netstat`
- list active TCP/UDP conn.	
	- routing table / port activity




