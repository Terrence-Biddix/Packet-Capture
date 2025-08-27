# Packet-Capture

Wireshark Packet Analysis Project
## Objective

The Wireshark Packet Analysis project focused on learning how to capture and analyze network traffic. The goal was to explore packet data, apply filters to identify relevant traffic, and investigate the details of network protocols. This hands-on experience was designed to build practical skills in traffic analysis, protocol inspection, and identifying key data flows within network communications.

### Skills Learned

- Proficiency in using Wireshark to capture and analyze network traffic.

- Ability to apply filters to isolate relevant packets for investigation.

- Understanding of network protocols including ICMP, TCP, UDP, HTTP, and DNS.

- Experience in examining packet structure from Frame, Ethernet, IP, and Transport layers.

- Strengthened analytical skills for identifying traffic patterns and interpreting payload data.

### Tools Used

- Wireshark – for packet capture and traffic analysis.

- Sample PCAP file – containing real-world browsing and DNS traffic.

- Filtering techniques – for isolating IP, MAC, DNS, and TCP traffic.

## Steps
*Ref 1: Exploring the Packet Capture File*

Opened the provided PCAP file in Wireshark to review captured traffic. Observed multiple types of traffic including DNS queries, TCP requests, and ICMP ping requests.

<img width="1865" height="685" alt="Packet capture 1" src="https://github.com/user-attachments/assets/02354724-09f4-4ac5-bbcb-f2fffb46bad9" />
<img width="933" height="689" alt="Packet Capture 2" src="https://github.com/user-attachments/assets/c1959dbf-5a13-4c6d-ad91-e0646ab3fed8" />


*Ref 2: Applying Basic Filters*

Used the filter ip.addr == 142.250.1.139 to view traffic between a client and a specific destination IP. This reduced the dataset to relevant communications only.
<img width="1335" height="830" alt="Packet Capture 3" src="https://github.com/user-attachments/assets/2e2abd00-d287-4ec0-99a1-0442076c0147" />





*Ref 3: Inspecting Protocol Layers*

Drilled down into a TCP packet to examine Frame, Ethernet II, IPv4, and TCP subtrees. Verified source and destination IP addresses, port numbers, and TCP flags.
<img width="1387" height="461" alt="Packet Capture 3 part 2" src="https://github.com/user-attachments/assets/446885fa-317d-4c76-a48c-867e6780df94" />
<img width="1190" height="413" alt="Packet Capture 3 part 3" src="https://github.com/user-attachments/assets/ed96a1d3-8882-4848-b693-2274df3b6f99" />
<img width="915" height="411" alt="Packet Capture 3 part 4" src="https://github.com/user-attachments/assets/40d7abb2-1246-404f-96fb-60db9cae2d57" />
<img width="950" height="433" alt="Packet Capture 3 part 5" src="https://github.com/user-attachments/assets/1ba626de-3872-47fa-b79e-a848c6bcdb0b" />





*Ref 4: DNS Traffic Analysis*

Applied the filter udp.port == 53 to analyze DNS query and response packets. Identified queries for opensource.google.com and verified the resolved IP address.

<img width="1378" height="585" alt="Packet Capture 7" src="https://github.com/user-attachments/assets/063c01f4-a9e5-4c51-a06f-0885383f4ef7" />
<img width="1864" height="744" alt="Packet Capture 7 part 2" src="https://github.com/user-attachments/assets/38ec3f95-d6ff-46ed-bf8f-387c03f5e1b1" />
<img width="1764" height="762" alt="Packet Capture 7 part 3" src="https://github.com/user-attachments/assets/5e7b4a12-ab0f-4fb6-a7a0-bcf9d649ecb8" />



*Ref 5: Inspecting TCP Traffic*

Filtered for HTTP traffic using tcp.port == 80. Examined packets to identify web requests, payload data, and session details. Applied advanced filter tcp contains "curl" to detect packets with specific text data in the payload.
(Insert screenshot showing HTTP request payload details)
<img width="1694" height="800" alt="Packet Capture 8" src="https://github.com/user-attachments/assets/ad3f16a0-96dc-4a69-b33c-b0f9570dd446" />
<img width="1106" height="555" alt="Packet Capture 8 part 2" src="https://github.com/user-attachments/assets/33f5c4e0-d746-4440-81b0-a3ddbf869d28" />
<img width="961" height="456" alt="Packet Capture 8 part 3" src="https://github.com/user-attachments/assets/bc893a8c-badf-45c8-a1ce-d4d21e65afc2" />
<img width="581" height="486" alt="Packet Capture 8 part 4" src="https://github.com/user-attachments/assets/e790a3c5-8f8a-44e8-ac41-40f0ddf13829" />
<img width="644" height="556" alt="Packet Capture 8 part 5" src="https://github.com/user-attachments/assets/c02b5ab0-6057-478e-875c-2f7ff4364dec" />
<img width="1366" height="412" alt="Packet Capture 9" src="https://github.com/user-attachments/assets/2864a981-5933-459f-bb4b-c7ecff031458" />



## Conclusion

This project provided practical experience in analyzing network traffic using Wireshark. By applying filters and drilling into protocol layers, I was able to:

- Open and interpret packet capture files.

- Identify source/destination IPs, ports, and protocols.

- Analyze DNS queries, HTTP traffic, and TCP payload data.

- Strengthen investigative skills necessary for cybersecurity monitoring and incident response.
