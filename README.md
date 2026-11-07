IT Help Desk Troubleshooting Lab

Project Overview

This project demonstrates my foundational IT support and networking skills through hands-on troubleshooting exercises using a Windows 11 computer.

The goal was to simulate common IT Help Desk situations, investigate technical problems, use Windows diagnostic tools, and document the results.


Skills Demonstrated

-Windows troubleshooting

-IP address configuration

-Network connectivity testing

-DNS troubleshooting

-Network route analysis

-CPU and RAM monitoring

-Command Prompt

-Technical documentation

Tools Used

-Windows 11

-Command Prompt (CMD)

-Ipconfig

-ping

-nslookup

-tracert

-Windows Task Manager

Scenario 1: IP Address Troubleshooting

Objective: Identify the computer’s IP configuration.

Command used:

*Ipconfig

Results:
-IPv4 Address: 192.168.0.154

-Subnet Mask: 255.255.255.0

-Default Gateway: 192.168.0.1

-Network Interface: Wi-Fi

Conclusion:

The computer had an IPv4 address and a default gateway assigned, indicating that the Wi-Fi interface had a usable local network configuration.



Scenario 2: Network Connectivity Troubleshooting

Objective: Test connectivity between the computer, its router, and an external IP address.

Commands used:
*ping 8.8.8.8 (Google public IP adress, external network)

*ping 192.168.0.1 (Router IP adress)

Results:

External IP test:

Packets sent: 4

Packets received: 0


Packet loss: 100%

Local router test:

Packets sent: 4

Packets received: 4

Packet loss: 0%

Average response time: 13 ms

Conclusion:

The computer successfully communicated with its local router but did not receive responses from Google’s public IP address. Further investigation was needed. A failed ping alone does not prove Internet access is unavailable because some networks block ICMP requests.


Scenario 3: DNS Troubleshooting

Objective: Determine whether the computer could translate a website name into an IP address.
Command used:

*nslookup google.com

Results:


DNS Server Address: 192.168.0.1

Domain queried: google.com

DNS resolution: Successful

Multiple IPv4 and IPv6 addresses returned.

Conclusion:
The DNS query successfully returned IP addresses for Google, demonstrating that DNS resolution was working during this test.


Scenario 4: Network Route Troubleshooting

Objective: Identify the network devices traffic passes through when attempting to reach an external destination.
Command used:

*tracert 8.8.8.8 (show the path data takes before reaching destination (8.8.8.8 which is google DNS )

Results:

Identified the local router at hop 1.

Identified additional network devices beyond the local router.

Received responses from several intermediate network devices.

Later hops returned request timeouts.

The destination was not confirmed as reached.

Conclusion:

The traceroute identified multiple network hops between the computer and the external destination. Some devices did not respond to traceroute probes. Further investigation would be needed to determine why the destination did not respond.


Scenario 5: Computer Performance Troubleshooting

Objective: Investigate CPU and RAM usage using Windows Task Manager.

*Tool used: Windows Task Manager.

Initial Results


Resource

Initial Usage

CPU

27%

Memory (RAM)

86%

Disk

1%

Google Chrome was using approximately:

CPU: 22.7%

Memory: 732.7 MB

Processes: 16

After Troubleshooting

After closing unnecessary applications and browser tabs, I checked Task Manager again.

Resource

Before

After

CPU

before 27%

before 3%

Memory (RAM)

before 86%

after 67%

Disk

before 1%

after 0%

Conclusion:

CPU usage decreased from 27% to 3%, while memory usage decreased from 86% to 67%.

This demonstrated how monitoring system resources and closing unnecessary applications can help reduce computer resource usage.


Key Takeaways

Through this project, I gained practical experience with:

-Identifying IP addresses, subnet masks, and default gateways.

-Testing network connectivity using ping.

-Understanding how DNS resolves domain names.

-Investigating network paths using traceroute.

-Monitoring computer performance using Task Manager.

-Documenting troubleshooting procedures and technical findings.

-Project Reflection

-This project helped me develop a better understanding of how IT support technicians investigate and troubleshoot common computer and networking problems.

-I learned the importance of testing one component at a time, analyzing command-line results, and documenting findings before making conclusions.

Future Improvements


-Practice DHCP troubleshooting.

-Investigate DNS failures in a controlled environment.

-Explore Windows Event Viewer.

-Practice Windows user account management.

-Build an Active Directory lab.

-Project Category: Information Technology / IT Support

-Operating System: Windows 11

-Project Type: Hands-on IT Troubleshooting Lab



























