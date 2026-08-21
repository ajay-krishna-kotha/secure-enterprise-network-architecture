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
- Suricata
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

## Key Technical Achievements

- Designed and implemented six isolated enterprise network segments for HR, Finance, IT, Server, Guest, and Management.
- Configured OPNsense as the central firewall and router with dedicated interfaces and subnets.
- Implemented least-privilege firewall policies controlling communication between departments.
- Configured DHCP services for automatic addressing across department networks.
- Deployed an internal enterprise server providing Apache, MySQL, and Samba services.
- Configured NAT and port forwarding to publish an internal web service.
- Configured a WireGuard VPN server, peer, dedicated VPN interface, and supporting firewall rules.
- Configured Unbound DNS with internal hostname resolution.
- Validated network segmentation using Kali Linux and Nmap.
- Troubleshot VMnet/interface mapping, firewall rules, routing, and connectivity issues.
  
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

 ## Security Validation

The network architecture was tested from individual department clients to verify that implemented firewall policies behaved as intended.

Connectivity and access-control testing included:

- `ping` for network reachability testing
- `netcat` for port-level connectivity testing
- `curl` for HTTP and internet-access verification
- `Nmap` for security validation and reconnaissance testing

A Kali Linux system placed within the restricted Guest network was used to test access to protected internal networks.

Nmap testing against the Server segment returned protected service ports as `filtered`, providing evidence that OPNsense was actively dropping unauthorized Guest-to-Server traffic.

## Project Limitations

The following areas were identified for further implementation and validation:

- End-to-end WireGuard connectivity from an external client was not completed.
- Full traffic-driven Suricata IDS/IPS alert validation was not completed.
- A dedicated DMZ for the externally published web server is recommended as a future improvement.
- Centralized logging and longer-term monitoring can be added in a future implementation.

## Project Report

The complete technical report documents the network design, implementation,
security controls, testing methodology, troubleshooting process, limitations,
and recommended improvements.

📄 [View Technical Project Report](docs/secure-enterprise-network-architecture-report.pdf)

## Disclaimer

This repository documents a cybersecurity project implemented in a
controlled virtual lab environment for educational and authorized
security-learning purposes.
