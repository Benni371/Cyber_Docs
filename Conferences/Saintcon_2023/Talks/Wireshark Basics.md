# Wireshark Basics
#### Speaker: Kyle Feuz
###### 26-10-2023
---
- How does sniffing work?
	- Promiscuous mode or port forwarding to sniff other computers traffic
	- Not going to see traffic your network doesnt see
- Know what normal traffic is like. Set up a baseline
- Find malicious traffic, troubleshooting, malware and forensic analysis
- Baseline
	- Use statistics tab on your file to see how your traffic is split up
		- conversations and endpoints
- How to sniff
	- Decrypting traffic (ssl_* files)
		- Edit -> preferences -> TLS
- General Capturing
	- Capture filters limit what you get obviously. You lose some data that you may need. If you filter out at this level you can miss it.
		- Use case is for very specific use cases when you want to capture traffic
	- Display filter is using port numbers so be wary if services are on uncommon ports
		- to capture all ssh, Preferences -> Protocols -> \[Protocol\] -> change ports
	- Filter buttons
		- Hit plus button at the end and give it a label