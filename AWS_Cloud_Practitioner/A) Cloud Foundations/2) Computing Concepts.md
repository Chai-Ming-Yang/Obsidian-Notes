**Servers:** 
- provide resources / services
- Resource redundancy (Memory & >1 CPU & Power Supply & Network Interfaces)
- types : [Web] [Database] [Mail] 
**security :** "made only be accessible on designated hardware"
- inaccessible over the internet

**Data Center**:
- physical location of organization data storage
- protect (failure / accidents)
- ideal condition to run
- [Servers] [Storage Device] [Network Device (router, switch)] 
  [Cooling Equipment] [Uninterruptable Power Supply (UPS)]
- On-Premise model  vs  Coud model

**Workflow** (Client Server Database):
1. Client sends request for web application
2. Web Server detects request
3. Web application accesses application data
4. Database server returns the application data
5. Web server returns an application webpage

**DBMS (Database Managent System):**


**Virtual Machines:**
- Scalable (resizable)
- has its own OS
- VM : fundamental unit of computing
Hypervisor : intermediate software layer (btw VM & resources) 
- (trap & process req)
- Latency (access hardware through hypervisor)
**Benefits:**
- Save Cost (Pay only used resources)
- Full Resource Utilization (reduced wastage)
- Reusability / Portability

EC2 (Elastic Compute) [VM]
AMI (Machine Image) [VM Image / Instance] 
S3 (Simple Storage Service)
Lambda (code exe) [serverless] [event driven] 


**SDLC**
1. Plan (defined goals & constraints)
2. Analyse [SRS] (risk, budget, time) 
3. Design 
4. Develop 
5. Test (unit, integration, security, performance)
6. Implement (staging deployment (test) --> deploy)
7. Maintain (corrective, adaptive) **80% of lifetime**

