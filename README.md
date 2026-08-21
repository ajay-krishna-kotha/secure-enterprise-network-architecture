# secure-enterprise-network-architecture
Secure enterprise network architecture designed with network segmentation, firewalling, IDS/IPS, VPN, and access-control principles using OPNsense.

## Overview

This project focuses on designing and implementing a secure network architecture for an enterprise environment.

The architecture applies defense-in-depth principles through network segmentation, firewall policies, IDS/IPS, secure remote access, and controlled communication between different network zones.

The project was developed in a controlled virtual lab environment using OPNsense and VMware Workstation.

## Objectives

- Design a secure enterprise network architecture.
- Segment different organizational departments and network zones.
- Control traffic between network segments using firewall rules and access controls.
- Implement IDS/IPS capabilities for network monitoring and threat detection.
- Provide secure remote access through VPN technologies.
- Reduce unauthorized access and lateral movement within the network.
- Document the architecture and security controls.

## Lab Environment

The project was implemented using a virtualized network environment.

### Platforms

- OPNsense
- Ubuntu Linux
- VMware Workstation

### Security & Networking Technologies

- Firewalls
- IDS/IPS
- VLANs
- Access Control Lists (ACLs)
- VPN
- NAT
- Network Segmentation
- TCP/IP

### Security Tools

- OPNsense
- Nmap
- Wireshark

## Architecture

The proposed architecture separates the enterprise environment into
different security zones and network segments.

The design considers:

- Internet / WAN
- Perimeter Security
- Internal LAN
- Departmental Network Segmentation
- Remote Employee Access
- Firewall-Controlled Communication
- IDS/IPS Monitoring

This approach limits unnecessary communication between network segments
and provides additional security controls between trusted and untrusted
networks.

## Security Controls

### Firewall

OPNsense was used as the primary firewall platform to control traffic
between network interfaces and security zones.

### Network Segmentation

Network segmentation was incorporated to separate different organizational
resources and reduce unnecessary communication between systems.

### IDS/IPS

Suricata was used with OPNsense to provide intrusion detection and
prevention capabilities.

### Secure Remote Access

VPN-based remote access was considered for securely connecting remote
employees to enterprise resources.

### Access Control

Firewall rules and access-control principles were used to restrict
communication based on network requirements.

## Implementation & Testing

The architecture was implemented in a controlled VMware environment.

Testing included:

- Network connectivity verification
- Firewall policy validation
- Network segmentation testing
- IDS/IPS configuration and monitoring
- Network reconnaissance using Nmap
- Traffic analysis using Wireshark

## Security Benefits

The architecture was designed to provide:

- Reduced attack surface
- Improved network isolation
- Controlled access between network segments
- Detection of suspicious network activity
- Secure remote connectivity
- Reduced potential for lateral movement
- Centralized firewall enforcement

## Key Learning Outcomes

Through this project, I developed practical understanding of:

- Enterprise network security architecture
- OPNsense firewall configuration
- Network segmentation
- Firewall rules and access control
- IDS/IPS implementation
- Suricata
- VPN concepts
- NAT and network communication
- Network troubleshooting
- Security architecture documentation

## Disclaimer

This repository documents a cybersecurity project implemented in a
controlled virtual lab environment for educational and authorized
security-learning purposes.
