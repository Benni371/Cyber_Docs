# Cloud Security
###### 10-01-2024
---
## General
- Users 
	- permissions policy, groups, access keys, passwords
- Roles
	- permission policy
	- should use these wherever possible
- All aws api's have tls 1.2 enabled on them so they are already encrypted
- Encryption at rest is an interesting topic for the cloud because the drives are stored in a highly secure facitlity that few people know the location of and is stored with 100s of other drives. Plus the data stored on your virtual disk is stored across multiple drives so stealing one drive would likely no give the attacker anything significant
## Cloud Security
- AWS Shared Responsibility Model
	- 