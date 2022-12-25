Network scanning tool
A more in depth list of the abilities of nmap: [nmap-cookbook](../../Resources/Nmap-CookBook.pdf)

### nmap \<ip-address\>
The simplest command possible.  The results show the detected ports on the ip-address

![[../../Images/BasicNmap.png|500]]


### nmap \<ip-address\> -p \<port\>
Scans a specific port

![[../../Images/NmapPort.png|500]]

Use -p "\*" to scan all ports 
![[../../Images/NmapAllPorts.png|500]]


### nmap \<ip-address\> -sV
Attempts to identify the vendor and software version for any open ports it detects

![[../../Images/NmapSV.png|500]]


### nmap \<ip-address\> -sC
The default script scan.  Script scans are typically used to detect vulnerabilities, discovering malware, or simply collecting more information from services.

![[../../Images/NMapSC.png|500]]


### nmap \<ip-address\> -PN
By default, before nmap attempts to scan a system for open ports it will first [ping](ping.md) the target to see if it is online. This feature helps save time when scanning as it causes targets that do not respond to be skipped.  This command tells it not to ping first and just go ahead and scan.

![[../../Images/NmapPN.png|500]]