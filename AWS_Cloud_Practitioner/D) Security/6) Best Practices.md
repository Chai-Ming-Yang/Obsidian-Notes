1. **No root account user**
	- remove root access key
2. **Require MFA**
3. **Activate AWS CloudTrail**
	- record all events
4. **Billing Report**
	- limit access to S3 bucket

## AWS Trusted Advisor
provide best practice in:
- Cost Optimization
- Performance
- Security
- Fault Tolerance
- Service Limits
Free Tier:
- IAM use                          MFA on root account
- security group                S3 bucket permissions
- check and notify if snapshots set public  *(RDS or EBS)*

### Post Authentication Tasks
- Restore IAM user permission
	- (accidental revoke of admin permission)

