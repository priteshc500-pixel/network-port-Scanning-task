# network-port-Scanning-task
1. find your local IP range:
    Windows CMD: IPCONFIG
    look for something like:
       IPv4 Address: 192.168.217.1
   Your network range is usually:
      192.168.217.1/24
   Run the scan: nmap -sS 192.168.217.1/24
   save output: nmap -sS 192.168.1.0/24 -oN scan_results.txt

   Interview Questions Answers
1. What is an open port?

An open port is a communication endpoint on a device that is actively accepting network connections. Services such as web servers, SSH, FTP, and databases use open ports to communicate with other devices.

2. How does Nmap perform a TCP SYN scan?

Nmap sends a SYN packet to the target port. If the target responds with SYN-ACK, the port is considered open. Nmap then sends an RST packet to terminate the connection without completing the TCP handshake.

3. What risks are associated with open ports?

Open ports can expose services to attackers. Vulnerable services may allow unauthorized access, data theft, malware infection, or remote code execution if not properly secured.

4. Explain the difference between TCP and UDP scanning.

TCP scanning checks connection-oriented services and is generally more reliable. UDP scanning checks connectionless services and is slower because UDP does not establish a connection before sending data.

5. How can open ports be secured?

Open ports can be secured by:
Closing unused ports
Using firewalls
Updating services regularly
Restricting access with ACLs
Using strong authentication
6. What is a firewall's role regarding ports?

A firewall monitors and controls incoming and outgoing network traffic. It can allow or block specific ports to protect systems from unauthorized access.

7. What is a port scan and why do attackers perform it?

A port scan is the process of discovering open ports and services on a target system. Attackers use port scanning during reconnaissance to identify potential entry points and vulnerabilities.

8. How does Wireshark complement port scanning?

Wireshark captures and analyzes network packets. It helps security professionals understand traffic patterns, verify scan results, troubleshoot network issues, and investigate suspicious activity.
