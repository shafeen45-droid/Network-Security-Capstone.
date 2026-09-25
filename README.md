# Final Capstone Project: Network Security Hardening Framework
**Submitted by:** Shafeen
**Course:** Compliance & Security Auditor Internship

## Project Overview
This repository contains the documentation, configuration blueprints, and hardening checklists compiled for the Final Capstone Project. The objective of this project is to research, design, and document practical enterprise network security practices—focusing on reducing the overall attack surface through access control optimization, network segmentation, perimeter filtering, and centralized monitoring.

## Core Architectural Implementations

### 1. Network Segmentation & Micro-Zoning
* Restructured flat broadcast topologies into dedicated Virtual Local Area Networks (VLANs).
* Implemented Layer-3 inter-zone Access Control Lists (ACLs) to strictly isolate user workstations from production database segments.
* Restrained the lateral threat propagation "blast radius" within localized network segments.

### 2. Access Control and Authentication Matrix
* Mandated Multi-Factor Authentication (MFA) across all administrative access vectors.
* Designed a Role-Based Access Control (RBAC) model to enforce the Principle of Least Privilege (PoLP).
* Outlined timed Privileged Access Management (PAM) windows for system modifications.

### 3. Perimeter & Traffic Inspection Infrastructure
* Configured Next-Generation Firewalls (NGFW) to enforce a strict default-deny policy on inbound and outbound pipelines.
* Integrated passive Intrusion Detection Systems (IDS) for baseline anomaly matching.
* Positioned inline Intrusion Prevention Systems (IPS) to automatically drop rapid-fire TCP SYN reconnaissance signatures in real time.

### 4. Device Hardening and Configuration Baseline
* Disabled legacy unencrypted management channels (Telnet, HTTP, SNMPv1) and updated to secure frameworks (SSHv2, HTTPS, SNMPv3).
* Enforced Layer-2 switch port security (MAC address filtering with a threshold constraint of 1).
* Streamed all system log events to a centralized SIEM platform for real-time telemetry analysis.

## Hardening Blueprint Checklist
- [x] Stateful Default-Deny Firewall Configuration
- [x] Multi-VLAN Network Segmentation Isolation
- [x] Multi-Factor Authentication (MFA) Deployment
- [x] Cleartext Protocol Deprecation (Telnet/HTTP to SSH/HTTPS)
- [x] Switch Port Security Validation
- [x] Centralized SIEM Telemetry Streaming Configuration
- [x] Automated Monthly Vulnerability Scan Lifecycle
