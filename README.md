# network-port-Scanning-task
1. find your local IP range:
    Windows CMD: IPCONFIG
    look for something like:
       IPv4 Address: 192.168.217.1
   Your network range is usually:
      192.168.217.1/24
   Run the scan: nmap -sS 192.168.217.1/24
   save output: nmap -sS 192.168.1.0/24 -oN scan_results.txt

Objective
Scan local network for open ports using Nmap.

Tools Used
Nmap
Wireshark

Command Used
nmap -sS 192.168.1.0/24

Findings
1.List detected hosts
2.List open ports
3.Services running

Security Risks
Explain risks of discovered ports

 Conclusion
This task helped me understand port scanning, TCP SYN scanning, and network reconnaissance.
