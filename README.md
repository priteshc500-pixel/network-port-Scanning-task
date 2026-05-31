# network-port-Scanning-task
1. find your local IP range:
    Windows CMD: IPCONFIG
    look for something like:
       IPv4 Address: 192.168.217.1
   Your network range is usually:
      192.168.217.1/24
   Run the scan: nmap -sS 192.168.217.1/24
   save output: nmap -sS 192.168.1.0/24 -oN scan_results.txt

