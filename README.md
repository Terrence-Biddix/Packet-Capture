# Packet-Capture

Wireshark Packet Analysis Project
## Objective

The Wireshark Packet Analysis project focused on learning how to capture and analyze network traffic. The goal was to explore packet data, apply filters to identify relevant traffic, and investigate the details of network protocols. This hands-on experience was designed to build practical skills in traffic analysis, protocol inspection, and identifying key data flows within network communications.

### Skills Learned

Proficiency in using Wireshark to capture and analyze network traffic.

Ability to apply filters to isolate relevant packets for investigation.

Understanding of network protocols including ICMP, TCP, UDP, HTTP, and DNS.

Experience in examining packet structure from Frame, Ethernet, IP, and Transport layers.

Strengthened analytical skills for identifying traffic patterns and interpreting payload data.

### Tools Used

Wireshark – for packet capture and traffic analysis.

Sample PCAP file – containing real-world browsing and DNS traffic.

Filtering techniques – for isolating IP, MAC, DNS, and TCP traffic.

## Steps
*Ref 1: Exploring the Packet Capture File*

Opened the provided PCAP file in Wireshark to review captured traffic. Observed multiple types of traffic including DNS queries, TCP requests, and ICMP ping requests.
(Insert screenshot of Wireshark overview with different colored packets)

*Ref 2: Applying Basic Filters*

Used the filter ip.addr == 142.250.1.139 to view traffic between a client and a specific destination IP. This reduced the dataset to relevant communications only.
(Insert screenshot showing filtered packets in Wireshark)

*Ref 3: Inspecting Protocol Layers*

Drilled down into a TCP packet to examine Frame, Ethernet II, IPv4, and TCP subtrees. Verified source and destination IP addresses, port numbers, and TCP flags.
(Insert screenshot of packet detail pane with expanded subtrees)

*Ref 4: DNS Traffic Analysis*

Applied the filter udp.port == 53 to analyze DNS query and response packets. Identified queries for opensource.google.com and verified the resolved IP address 142.250.1.139.
(Insert screenshot of DNS query and answer details)

*Ref 5: Inspecting TCP Traffic*

Filtered for HTTP traffic using tcp.port == 80. Examined packets to identify web requests, payload data, and session details. Applied advanced filter tcp contains "curl" to detect packets with specific text data in the payload.
(Insert screenshot showing HTTP request payload details)

## Conclusion

This project provided practical experience in analyzing network traffic using Wireshark. By applying filters and drilling into protocol layers, I was able to:

Open and interpret packet capture files.

Identify source/destination IPs, ports, and protocols.

Analyze DNS queries, HTTP traffic, and TCP payload data.

Strengthen investigative skills necessary for cybersecurity monitoring and incident response.
