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
### AWS Shared Responsibility Model
- Security OF the cloud (AWS)
	- Physical security of data centers
	- Hardware and software infra
		- intrusion detection
	- Network and Virtualization infra
		- instance isolation
- Security IN the cloud (Customer)
	- responsible for the services that you deploy including patching and maintenance
	- Applications; passwords, role-based access
	- OS or hostbased firewalls
	- Network conf and account management
	- Customer is in control of their data
### AWS IAM
- used to manage access to aws resources
	- **Who** can access the resource
	- **Which** resources can be accessed and what can the user do to the resource
	- **How** resources can be accessed
- Components
	- a person or app can auth with an aws account
		- Programmatic access
			- access key ID
			- secret access key
		- AWS Console
			- password, user name and account ID, mfa (optional)
	- a group is a collection of users that are granted identical authorization
	- a policy is a document that defines which resources can be accessed and the level of access to each resource
		- identity based policy
			- attach to any IAM entity
			- deny statements always win
	- a role is a mechanism to grant a set of permissions for making aws service requests. Similar to using `sudo`
- Authorization
	- all permissions are implicitly denied by default
	- looks first for permission explicitly denied
### Securing a New AWS Account
- do not use rot user. create a privileged user
- enable mfa for root
- create a group for admin acccess
- remove root account access keys