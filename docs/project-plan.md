# Project Plan

## Project Name

Secure Linux Bastion Host on AWS

---

## Project Overview

This project focuses on designing, deploying, and hardening a Linux Bastion Host in AWS.

The Bastion Host serves as a controlled administrative entry point into cloud infrastructure, reducing the exposure of critical systems while enforcing secure access controls.

The project follows DevSecOps principles by integrating security directly into infrastructure deployment, configuration, and validation.

---

## Business Problem

Organizations often expose administrative services directly to the internet.

This increases the risk of:

- Unauthorized access
- Credential theft
- Brute-force attacks
- Lateral movement within environments
- Misconfigured infrastructure

A Bastion Host reduces this attack surface by centralizing administrative access through a hardened and monitored entry point.

---

## Project Objectives

### Infrastructure

- Deploy Ubuntu EC2 Instance
- Configure Secure SSH Access
- Configure AWS Security Groups

### Security

- Restrict SSH Access
- Implement UFW Firewall
- Apply System Updates
- Minimize Attack Surface

### Documentation

- Create Architecture Diagram
- Document Security Controls
- Record Deployment Steps
- Produce Security Assessment Report

### Validation

- Verify SSH Connectivity
- Verify Firewall Rules
- Validate Security Group Configuration
- Verify System Hardening

---

## Threat Model

The project is designed to reduce risks associated with:

### External Threats

- Internet-wide SSH scanning
- Brute-force attacks
- Credential stuffing
- Unauthorized access attempts

### Internal Threats

- Excessive permissions
- Weak configurations
- Untracked administrative access

---

## Success Criteria

The project will be considered successful when:

- EC2 Instance is deployed successfully
- SSH access is functional
- Security Group restrictions are enforced
- UFW firewall is active
- Security controls are documented
- Validation checks are completed

---

## Project Status

Current Phase:

Documentation and Planning

Next Phase:

Infrastructure Hardening
