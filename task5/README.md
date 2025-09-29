## Task 5: Capture and Analyze Network Traffic Using Wireshark

**Objective:**  
Capture live network packets using Wireshark and analyze the protocols involved in communication.

**Steps Performed:**  
1. Installed and launched Wireshark.  
2. Started packet capture on the active network interface.  
3. Generated traffic by browsing a website and using the `ping` command.  
4. Stopped capture after ~1 minute and saved the file as `.pcapng`.  
5. Applied filters (`dns`, `tcp`, `icmp`) to analyze specific traffic.  

**Protocols Identified:**  
- **DNS:** Queries and responses for domain name resolution.  
- **TCP:** Reliable connections established (3-way handshake observed).  
- **ICMP:** Ping packets used for connectivity testing.  
- **(Optional) ARP:** Local address resolution packets.  

**Outcome:**  
- Successfully captured and analyzed live network traffic.  
- Gained hands-on experience with packet inspection and protocol behavior.  
- Deliverables:  
  - Packet capture file (`wireshark_capture.pcapng`)  
  - Short analysis report  