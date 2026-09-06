# Week 3 — Task 9: Network Traffic Analysis — Wireshark Basics

![Cyber Security](https://img.shields.io/badge/Domain-Cyber%20Security-red)
![Task](https://img.shields.io/badge/Internship-Week%203%20%7C%20Task%209-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Project Overview

This project covers the fundamentals of network traffic analysis using Wireshark and packet capture data.

Network traffic analysis is an important SOC skill because security analysts need to understand packets, protocols, IP addresses, DNS requests, HTTP traffic, TCP connections, and potentially suspicious network activity.

The practical work completed for this task includes:

- Opening and examining a packet capture
- Understanding packets and protocols
- Using IP address filters
- Filtering DNS traffic
- Filtering HTTP traffic
- Filtering TCP traffic
- Inspecting packet information
- Understanding plaintext data exposure
- Completing the required TryHackMe learning activity

## Objectives

1. Capture or analyze network traffic.
2. Understand basic packet structure.
3. Use Wireshark display filters.
4. Analyze IP-address-based traffic.
5. Identify DNS traffic.
6. Identify HTTP traffic.
7. Inspect an HTTP request packet.
8. Understand how plaintext information can be exposed.
9. Document the practical work with screenshots.

## Practical Work

### Packet Capture

The packet capture used during the practical analysis was:

```text
MCPE-0.15.pcapng
```

The capture contained approximately 120 packets.

Packet captures provide a record of network communication that can be examined during security investigations.

An analyst can inspect information such as:

- Source IP
- Destination IP
- Source port
- Destination port
- Protocol
- Packet length
- TCP flags
- DNS queries
- HTTP requests
- HTTP responses

## Wireshark Display Filters

Display filters allow an analyst to narrow down a large packet capture and focus on specific traffic.

### IP Address Filter

```text
ip.addr == 192.168.1.6
```

This filter displays packets where `192.168.1.6` is either the source or destination IP address.

### DNS Filter

```text
dns
```

This filter displays DNS-related packets.

### HTTP Filter

```text
http
```

This filter displays HTTP traffic and allows HTTP requests and responses to be investigated.

### TCP Filter

```text
tcp
```

This filter displays TCP traffic.

## Network Traffic Concepts

### IP Addresses

IP addresses identify hosts participating in network communication.

During an investigation, filtering traffic by IP address can help an analyst determine what a specific host is communicating with.

### DNS

DNS converts domain names into IP addresses.

DNS traffic can be useful during investigations because suspicious domains, unusual lookups, and repeated DNS requests may provide indicators of compromise.

### HTTP

HTTP is an application-layer protocol used for web communication.

Unencrypted HTTP traffic can expose information transmitted between systems, making it important for SOC analysts to inspect when investigating suspicious traffic.

### TCP

TCP provides reliable communication between network hosts.

TCP analysis can help identify connections, ports, communication patterns, and application traffic.

## HTTP Request Analysis

An HTTP packet was inspected during the practical exercise.

A SOC analyst can examine:

- Source IP
- Destination IP
- Source port
- Destination port
- HTTP method
- Host
- Request URI
- User-Agent
- Packet data

For example:

```text
GET / HTTP/1.1
Host: example.com
```

Because HTTP is not encrypted by default, packet inspection can potentially reveal information transmitted between the client and server.

## Understanding Suspicious Network Traffic

Potential indicators that may require further investigation include:

- Unexpected external IP addresses
- Repeated connections to an unfamiliar destination
- Unusual destination ports
- Large amounts of unexpected traffic
- Suspicious DNS queries
- Communication with known malicious infrastructure
- Cleartext credentials
- Unusual HTTP requests
- Repeated failed connections

These indicators should be correlated with other security data before determining whether an event is malicious.

## SOC Analyst Relevance

Packet analysis is useful when investigating:

- Suspicious IP addresses
- Unexpected network connections
- Malware communication
- Command-and-control traffic
- Suspicious DNS requests
- Unencrypted HTTP traffic
- Possible credential exposure
- Unusual ports and protocols
- Data exfiltration investigations
- Incident response

A SOC analyst can use packet captures as additional evidence alongside endpoint logs, firewall logs, DNS logs, authentication logs, proxy logs, and SIEM alerts.

## Evidence

Screenshots are stored in the `Report/` directory:

- `w1.png`
- `w2.png`
- `w3.png`
- `w4.png`
- `w5.png`

## Repository Structure

```text
Week-3-Task-9-Network-Traffic-Analysis-Wireshark-Basics/
│
├── README.md
├── Week-3-Task-9-Network-Traffic-Analysis-Wireshark-Basics.pdf
│
└── Report/
    ├── report.md
    ├── w1.png
    ├── w2.png
    ├── w3.png
    ├── w4.png
    └── w5.png
```

## Full Report

[Full report: Report/report.md](report/report.md)
