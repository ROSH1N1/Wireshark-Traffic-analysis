# Wireshark Traffic Analysis

## Overview

This project demonstrates the capture and analysis of network traffic using Wireshark on Kali Linux. The objective was to identify common network protocols, examine packet flows, and understand how devices communicate over a network.

## Objectives

* Capture live network traffic.
* Identify commonly used network protocols.
* Analyze packet communication patterns.
* Understand how DNS resolution and encrypted communication work.
* Document findings from captured traffic.

## Tools Used

* Wireshark
* Kali Linux

## Methodology

### 1. Traffic Capture

Network traffic was captured using the wireless network interface (`wlan0`) while browsing various websites and online services.

### 2. Protocol Analysis

Captured packets were filtered and analyzed using Wireshark display filters to identify different protocols and communication patterns.

The following filters were used:

| Filter | Purpose                           |
| ------ | --------------------------------- |
| dns    | Analyze DNS queries and responses |
| tcp    | Analyze TCP communication         |
| tls    | Analyze encrypted TLS traffic     |
| quic   | Analyze QUIC protocol traffic     |

## Findings

### DNS Analysis

DNS traffic was observed while resolving domain names into IP addresses.

Examples observed:

* chatgpt.com
* google.com
* web.whatsapp.com

**Observation:** DNS queries and responses allow devices to locate internet services before establishing connections.

---

### TCP Analysis

TCP packets were identified during communication with remote servers.

**Observation:**

* Reliable communication was established using TCP.
* Acknowledgment packets confirmed successful packet delivery.
* HTTPS traffic commonly used destination port 443.

---

### TLS Analysis

TLS traffic was identified during secure web browsing sessions.

**Observation:**

* TLSv1.2 encrypted communications were detected.
* Packet contents were protected through encryption.
* Secure communication was established between client and server.

---

### QUIC Analysis

QUIC traffic was observed while accessing modern web applications.

**Observation:**

* QUIC operates over UDP port 443.
* Provides faster and secure communication.
* Commonly used by modern browsers and web services.

## Results

The captured network traffic contained multiple protocols including:

* DNS
* TCP
* TLSv1.2
* QUIC

The analysis demonstrated how modern applications establish secure connections, resolve domain names, and exchange data across networks.

## Conclusion

Successfully captured and analyzed live network traffic using Wireshark. Identified common network protocols, examined packet flows, and documented communication patterns. This project improved understanding of network communication, packet analysis, and protocol behavior in real-world environments.

## Screenshots

The screenshots folder contains packet captures demonstrating:

* DNS traffic analysis
* TCP packet analysis
* TLS encrypted communication
* QUIC protocol communication

## Author

Roshini U
