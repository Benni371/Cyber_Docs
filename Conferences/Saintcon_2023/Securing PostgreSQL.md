# Alice, this is Bob: A Deep Dive into Database Security with PostgreSQL
#### Speaker: Roberto Mello
###### 26-10-2023
---
- Database Security
	- Who can access, auth?
		- Host based auth (pg_hba.conf)
		- Ideal is kerberos auth, ssl certs or scram-sha-256
			- ldap, radius, password aren't great methods
		- Use GRANT command to tell users what they can use
	- What can they access, change?
	- who did what when?
	- Who can access backups?
	- How can I recover?