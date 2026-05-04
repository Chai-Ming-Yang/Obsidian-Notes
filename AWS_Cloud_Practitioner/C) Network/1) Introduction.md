##### Computer Network
- >1 devices  Logically Connected
- Communicate  &  Share Resources
##### Port Number *(25565)*
- Paired with IP together to uniquely identify a source


# OSI Model
| Layer           |                                                                                |
| --------------- | ------------------------------------------------------------------------------ |
| 1. Physical     | Transmit over physical network<br><br>                                         |
| 2. Data Link    | Define format of data on network<br>**Frame** *(assoc w. MAC Address)*<br><br> |
| 3. Network      | Decide Physical path taken<br>**Packet** (assoc w. IP Address)<br><br>         |
| 4. Transport    | *Establish Logical Connection* *Src & Dst*<br>TCP  &  UDP<br><br>              |
| 5. Session      | *Unique ID* to data from Application Layer<br><br>                             |
| 6. Presentation | *Data Format*<br><br>                                                          |
| 7. Application  | *Interface* to access network<br><br>                                          |

# Components
|                      |                                                                                                                                   |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Client**           | Make requests to server<br><br>                                                                                                   |
| **Server**           | Responds to request from client<br><br>                                                                                           |
| **NIC**              | Chip to connect to internet<br>**MAC Address** assigned to card<br>  - Identifier Sender & Receiver<br>  - *Physical Address*<br> |
| **Network<br>Cable** | Physically Connect >1 Networks<br>Fiber-Optics<br>Twisted-Pair *(Ethernet Cable)*<br><br>                                         |
| **Router**           | Connect >1 network *(switch)* by IP<br>**Layer 2 & 3**<br>Block unauthorized port<br><br>                                         |
| **Switch**           | Connect >1 node by MAC Address<br>**Layer 2**<br>Prevent data collision<br>                                                       |
| **Modem**            | Connect Internet (ISP)                                                                                                            |
| Node<br>**NIC**      | <br><br>                                                                                                                          |
| **LAN**              | Local Area Network<br>Each Router represents a LAN<br><br>                                                                        |
| **WAN**              | Wide Area Network<br>Connect >1 LAN<br><br>                                                                                       |

# Topology
|            |                                                                                       |
| ---------- | ------------------------------------------------------------------------------------- |
| **Bus**    | **1** Backbone Cable<br>- monodirectional<br>- **1** signal at a time (from any node) |
| **Star**   | 1 Central switch<br>- Data sent pass thru central node                                |
| **Mesh**   | Peer to Peer connection `(N!)`<br>- expensive                                         |
| **Hybrid** | >1 topologies                                                                         |
Physical --> Physical Wires & Connections
Logical  --> How data moves through network

|                                         |                                                                                                                                       |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **Amazon VPC**<br>Virtual Private Cloud | **Virtual Network**<br>*(Virtual Wiring)*<br>SDN *(Software-defined networking)*<br>"No need manual plug device"<br>--> `SCALABILITY` |
| **VPC Peering**                         | Connect >1 VPC                                                                                                                        |

## LAN
| Client-Server Model                                                         | Peer-Peer Model                                                                       |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| Data Mgmt & Hosting<br>- Centralized at server<br>*Single Point of Failure* | Share tasks & workload<br>- among peers                                               |
|                                                                             | - Backup each node<br>- non-restrictive security requirements<br>- limited peers used |
## Network Protocol
| Connection-Oriented                                                                                                            | Connection-less                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| Create session *(sender/receiver)*<br> - Overhead<br>**"Synchronous"**<br> - real-time feedback<br> - continuous data transfer | No Session<br> - no overhead *(fast)*<br>**Asynchronous**<br> - Delayed receiving<br> - no feedback |
- Layer 3 & 4
#### Examples of Network Protocol
|                                           |                                                                                                                                                                         |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **IP *(Internet Protocol)***              | Routing rules                                                                                                                                                           |
| **TCP *(Transmission Control Protocol)*** | Reliable, Connection-oriented delivery<br> - TCP handshake *(3-step)*<br>  `(SYN)  (SYN/ACK)  (ACK)`<br>  `(FIN)  (FIN/ACK)  (ACK)`<br>  `(RST)` "conn. close abruptly" |
| **TCP/IP**                                | Combine TCP & IP                                                                                                                                                        |
| **UDP *(User Datagram Protocol)***        | Connection-less Communication<br> - Speed   *(streaming)*                                                                                                               |
