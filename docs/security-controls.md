# Security Controls

## Overview

This document outlines the security controls implemented within the Secure Linux Bastion Host project.

The objective is to reduce the attack surface, restrict unauthorized access, and align with DevSecOps security practices.

---

# Control 1: AWS Security Groups

## Purpose

Control inbound and outbound traffic at the instance level.

## Implementation

Inbound Rules:

- SSH (22/TCP)
- Source: My Public IP Only

Outbound Rules:

- Allow All Outbound Traffic

## Security Benefit

Restricts administrative access to approved sources and reduces exposure to internet-wide scanning.

---

# Control 2: SSH Access Control

## Purpose

Provide secure remote administration.

## Implementation

- SSH Key Authentication
- No Password-Based Login
- Ubuntu Default User

## Security Benefit

Reduces risk of brute-force attacks and credential theft.

---

# Control 3: UFW Firewall

## Purpose

Provide host-level firewall protection.

## Implementation

- UFW Enabled
- SSH Allowed
- All Unnecessary Ports Blocked

## Security Benefit

Creates a second security boundary beyond AWS Security Groups.

---

# Control 4: System Updates

## Purpose

Reduce exposure to known vulnerabilities.

## Implementation

Commands:

sudo apt update

sudo apt upgrade -y

## Security Benefit

Ensures security patches are applied.

---

# Control 5: Least Privilege

## Purpose

Limit administrative access.

## Implementation

- Dedicated Administrative User
- Restricted Access Paths

## Security Benefit

Reduces impact of compromised accounts.

---

# Control 6: Logging and Monitoring

## Purpose

Track administrative activity.

## Implementation

- Linux Authentication Logs
- SSH Login Tracking
- System Logs

## Security Benefit

Provides visibility into access attempts and security events.

---

# Security Review Status

| Control | Status |
|----------|----------|
| Security Groups | Implemented |
| SSH Keys | Implemented |
| UFW Firewall | Pending |
| Updates | Pending |
| Least Privilege | Pending |
| Logging | Pending |
