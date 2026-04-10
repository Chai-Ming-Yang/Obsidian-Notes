Buckets == Folder
Objects == File
## Buckets 
- Data stored as **objects** inside **buckets**
- 1 object max 5 TB
- **11 9s** 
	- (99.999999999%) durability
- Customer have granular access to buckets
- **Globally UNIQUE** bucket name
- **UNIQUE** object-key
### Object-Level storage
- change a part of the file 
- reupload entire file

### Considerations:
1. amount of storage
2. Request
	- GET (read permissions)
	- PUT (write permissions)
	- COPY (GET + PUT)
3. Data Transfer
	FREE
	- Transfer into S3
	- same region CloudFront / EC2
	PAID
	- Transfer out
	- diff region

## Amazon S3
**FREE** upload   &   transfer to (EC2/CloudFront) of same region 
**PAID** download (PUT/GET request) HTTP(s)   &   Transfer to other region
storage sized scaled automatically
optional encryption
data is private on default
redundancy (bucket copied over 3AZ in same region)
### Standard
- frequent accessed (1000/day)
- static website cheap alternative
- 11 9s durability
- 4 9s availability
### Intelligent Tiering
- Transitions between **Standard** and **Standard-IA**
	- if data not accessed within 30 days
	- Transition is free
### Standard-IA (Infrequent Access)
- cheaper than standard
- expensive & slow (hours) to retrieve
- infrequent accessed (1-2/month)
- 11 9s durability
- 3 9s availability
- "Government files"
### One Zone-IA (Infrequent Access)
- not stored redundantly (possibility loss file)
- store easily re-creatable data
### Glacier
- Archive & Backup
- Disaster Recovery
- Quarterly accessed
### Glacier Deep Archive
- retention period: 180 days minimum
- scared to delete


## Tools
### AWS Management Console
- 
### CLI
- 
### SDK 
- 
### REST endpoints
- user can access with URL
- `{region-code}-amazon.com/{bucket-name}/`
