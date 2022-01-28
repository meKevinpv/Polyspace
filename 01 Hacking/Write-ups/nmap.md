Status: #Doing
Tags: #Writeup #Hacking #nmap
Links: [[Environment - Hacking]]
MOC: [[Hacking MOC]]
___
# Writeup - nmap
Nmap is an **open-source** tool for network exploration.

Nmap can detect:
- Running applications
- Operating systems
- Packet filters/firewalls
- etc.

## Port scanning
Nmap can detect 4 different states a port is in
- Open
- Closed
- Filtered
	- This means there is a firewall, filter or other network obstacle blocking the port.
- Unfiltered
	- This means the port responds to nmap but it still cannot determine weather it is open or closed.


## Nmap options
Nmap has several different options that can be used, here I put the most relevant ones:
- Target specification
	- Targetting multiple targets based on a file `-iL <filename>`
- Host discovery
	- No ping, treat all hosts as active `-Pn`.
		- This does some interesting things, first off it will always scan every IP. Secondly, it slows down the scan because default timing parameters are used to make sure there is time to respond. Thirdly, if you want to skip host discovery *and* port scanning use `-Pn -sn`.
	- No [[DNS resolution]] `-n`
	- Always [[DNS resolution]] `-R`, fun to combine with `--resolve-all` which scans each resolved adress.
- Scanning techniques
- Port specification
- Service/Version detection
- Script scan
- OS Detection
- Timing and performance
- Firewall/IDS evasion and spoofing
- Output
- Misc.