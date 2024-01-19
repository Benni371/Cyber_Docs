# Intro and RAM Forensics
###### 18-01-2024
---
## General
- Good certs for forensics 
	- GIAC GCFA, GCFE, EnCASE cert
- NSRL (National Software Reference List)
	- list of known good software hashes
## RAM Forensics
- First things we do on a captured computer
	- Identify if the volume is encrypted or not
		- Encrypted Disk Detector (EDD) looks for bitlocker and other encryption technologies. Can help so you know what to target in the RAM
	- Check the OS Version that is currently running
	- Capture RAM
		- **the encryption keys are in the RAM!!!!!**
- Knowing what things were running during the time of the arrest is very critical
- RAM is critical for detecting malware
- Volatility commands
	- Shellbags