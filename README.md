# elevateday5task
task5
# Network Traffic Analysis with Wireshark

A comprehensive network packet capture and analysis project demonstrating protocol identification, traffic filtering, and security assessment using Wireshark.

## 📋 Project Overview

This project captures and analyzes live network traffic to identify basic protocols and traffic patterns. Using Wireshark as the primary network protocol analyzer, the analysis covers multiple network layers and provides insights into normal network behavior.

## 🎯 Objectives

- Capture live network packets using Wireshark
- Identify and analyze various network protocols
- Demonstrate traffic filtering and classification techniques
- Document network communication patterns
- Assess security implications of captured traffic

## 🛠️ Tools Used

- **Wireshark** - Network Protocol Analyzer
- **Network Interface** - Live packet capture
- **PCAPNG Format** - Next Generation packet capture format

## 📊 Capture Summary

| Metric | Value |
|--------|-------|
| **Capture Duration** | ~1 minute |
| **Total Packets** | 189 packets |
| **Capture File** | `network_capture_task5.pcapng` |
| **Local IP** | 10.0.2.15 |
| **Analysis Depth** | Layer 2-7 protocols |

## 🔍 Protocols Identified

### 1. DNS (Domain Name System)
- **Layer**: Application
- **Purpose**: Domain name resolution
- **Traffic**: 10.0.2.15 ↔ 10.0.2.3
- **Query Types**: A, AAAA, PTR records
- **Packet Size**: 73-137 bytes

### 2. ICMP (Internet Control Message Protocol)
- **Layer**: Network
- **Purpose**: Network diagnostics and connectivity testing
- **Traffic**: 10.0.2.15 ↔ 157.240.237.174
- **Packet Size**: 98 bytes
- **Function**: Echo requests/replies (ping)

### 3. TCP (Transmission Control Protocol)
- **Layer**: Transport
- **Purpose**: Reliable connection-oriented communication
- **Features**: Connection establishment, data transfer
- **Ports**: Various standard web ports observed

### 4. ARP (Address Resolution Protocol)
- **Layer**: Data Link
- **Purpose**: MAC address resolution
- **Packet Size**: 64 bytes
- **Function**: IP to MAC address mapping

## 🔬 Analysis Techniques

### Filtering Methods Applied
- Protocol-specific filtering (`dns`, `icmp`, `tcp`)
- Source/destination IP filtering
- Packet size analysis
- Time-based traffic examination

### Traffic Patterns Observed
- Local to remote server communication
- Frequent DNS lookups for domain resolution
- Mixed protocol usage typical of web browsing
- Proper protocol layering and interaction

## 🛡️ Security Assessment

### Key Findings
✅ Normal network behavior patterns observed  
✅ No suspicious or malicious traffic detected  
✅ Standard protocol implementations  
✅ Proper DNS resolution sequences  
✅ Legitimate ICMP usage for diagnostics  

## 📁 Project Structure

```
network-analysis/
├── network_capture_task5.pcapng    # Packet capture file
├── wireshark_analysis_report.txt   # Detailed analysis report
└── README.md                       # This file
```

## 🚀 Skills Demonstrated

- [x] Wireshark installation and configuration
- [x] Live packet capture techniques
- [x] Multi-protocol identification and analysis
- [x] Advanced traffic filtering and classification
- [x] Network security assessment
- [x] Technical documentation and reporting
- [x] Protocol stack understanding (OSI layers 2-7)

## 📈 Key Insights

1. **Protocol Diversity**: Successfully identified 4+ different network protocols
2. **Layer Analysis**: Comprehensive coverage from Data Link to Application layers
3. **Traffic Characterization**: Normal browsing patterns with proper protocol behavior
4. **Security Posture**: No anomalous or suspicious network activity detected

## 🔧 Technical Details

- **Capture Interface**: Primary network interface
- **File Format**: PCAPNG (Packet Capture Next Generation)
- **Analysis Scope**: Full packet inspection and protocol dissection
- **Documentation**: Comprehensive technical reporting

## 📝 Usage

1. **Open Wireshark** and load the capture file
2. **Apply filters** to focus on specific protocols or traffic
3. **Analyze packets** using the detailed report as reference
4. **Review findings** for network behavior patterns

## 🎓 Learning Outcomes

This project demonstrates practical network analysis skills including:
- Understanding of network protocol hierarchies
- Proficiency with industry-standard analysis tools
- Ability to identify normal vs. anomalous network behavior
- Technical documentation and reporting capabilities

## 📄 Documentation

- **Full Analysis Report**: `wireshark_analysis_report.txt`
- **Capture File**: `network_capture_task5.pcapng`
- **Protocol Reference**: Detailed breakdown of each identified protocol

## 🏷️ Tags

`wireshark` `network-analysis` `packet-capture` `cybersecurity` `protocols` `dns` `tcp` `icmp` `arp` `network-security`

