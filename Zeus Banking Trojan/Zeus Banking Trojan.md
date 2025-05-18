# Zeus Banking Trojan

This section focuses on analyzing the Zeus Banking Trojan. We begin with background information and an overview of the tools used. The analysis workflow includes provisioning a secure lab, acquiring and labeling the malware sample, and conducting both static and dynamic analysis. The process concludes with detailed reporting and identification of indicators of compromise (IOCs). It targets banking credentials and financial data using stealthy techniques like keylogging and form grabbing. Zeus is recognized for its persistence and ability to evade detection while exfiltrating sensitive user information.

# Infection Vectors
- Phishing Emails (Social Engineering)
- Drive-by Downloads

# Downloading the Malware
Previously, the two VMs were configured for isolated communication to prevent external network access. To download the Zeus Trojan, temporarily connect the FlareVM to the internet by switching its network adapter to NAT mode in VMware. 

Downloaded it from here:
https://github.com/ytisf/theZoo/tree/master/malware/Binaries/ZeusBankingVersion_26Nov2013

# Analysis
## Basic Analysis

Checked for suspicious file with VirusTotal. Concluded that **62/75 security vendors had flaged it as malicious**.

![virustotal scan](https://github.com/SMUGLER79/MalScan---Malware-Analysis-Lab/blob/main/Zeus%20Banking%20Trojan/virustotal.jpg)
