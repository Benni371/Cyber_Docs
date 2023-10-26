# Alice, this is Bob: A Deep Dive into Database Security with PostgreSQL
#### Speaker: Roberto Mello
###### 26-10-2023
---
- Database Security
	- Basic Policies
		- Host based auth (pg_hba.conf)
		- Ideal is kerberos auth, ssl certs or scram-sha-256
			- ldap, radius, password aren't great methods
		- Use GRANT command to tell users what they can use
		- STIG comprehensive guide for secure configuration
		- PGCrypto, PostgreSQL Anonymizer
	- SuperUser Control?
			- set_user extension helps disable superuser permissions
	- Logging
		- Database logs
		- sensible logging policies
		- PGAudit Extension
			- detailed session object logging
			- logs for compliance