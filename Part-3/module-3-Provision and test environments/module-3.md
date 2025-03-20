# Provision and Configure Target Environments

## Overview
This document provides a summary of provisioning and configuring target environments for software deployment, focusing on Continuous Delivery and Infrastructure as Code (IaC).

## Key Concepts

### 1. Release Pipeline Deployment
- Deploys software to target environments.
- Incorporates Infrastructure as Code (IaC) for Continuous Delivery.

### 2. Target Environments
#### On-Premises Servers
- Pre-configured hardware and OS.
- Focus on application deployment.
- Scripts for server management stored in source control.
- PowerShell DSC for server state management.

#### Infrastructure as a Service (IaaS)
- Cloud-based servers (e.g., Virtual Machines, networks).
- IaC for creating servers and components.
- Tools like Azure Resource Manager for on-demand infrastructure.

#### Platform as a Service (PaaS) & Functions as a Service (FaaS)
- Cloud-managed infrastructure (e.g., Azure SQL Database, Azure Functions).
- User deploys application; cloud handles infrastructure.
- Templates (e.g., Azure Resource Manager) define infrastructure.

#### Clusters
- Group of servers for high-scale applications.
- Managed clusters (PaaS) or self-managed (IaaS).
- Container clusters (e.g., AKS) for containerized applications.

#### Service Connections
- Required for pipeline access to resources.

### 3. Infrastructure as Code (IaC)
- Essential for Continuous Delivery.
- Infrastructure creation/configuration integrated into the release pipeline.
- Scripts/templates stored in source control alongside application code.

### 4. Tools and Technologies
- **PowerShell DSC**: Maintains server state.
- **Azure Resource Manager**: Creates infrastructure on demand.
- **Azure CLI/Command-Line Tools**: Define infrastructure templates.

## Summary
- Infrastructure creation/configuration should be part of the release pipeline.
- IaC enables on-demand server and environment creation, supporting Continuous Delivery.