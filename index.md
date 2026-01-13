---
title: Introduction
layout: home
nav_order: 1
---

# TechWorkshop L300 - Migrate and modernize workloads to Azure - Linux and PostgreSQL

## Overview

In this lab, you'll plan and execute a migration of a representative Linux workload from an on-premises datacenter to **Microsoft Azure**. You'll use **Azure Migrate** to discover and assess the environment, choose modernization paths, and then migrate both a database tier (PaaS) and an application tier (IaaS). Finally, you'll apply post-migration operational controls for security, backup, monitoring, and cost governance.


## Case study: Linux Migrate
**Terra Firm Laboratories** is a global bioengineering company and a leading researcher in genetic and biological science technology. Founded in 1975, Terra Firm's headquarters are in Palo Alto, CA. Mission-critical workloads are currently hosted in an on-premises datacenter, and the organization is beginning a journey to modernize and migrate into the cloud using Microsoft Azure.

The CTO, **Dennis Nedry**, has initiated an effort to adopt Azure and modernize infrastructure by reducing technical debt and streamlining operations using **Infrastructure as a Service (IaaS)** and **Platform as a Service (PaaS)** capabilities. Terra Firm completed an initial analysis across more than 250 workloads and selected one workload to validate the migration plan end-to-end. The environment includes multiple Linux distributions (RHEL, SUSE, Ubuntu, and a Debian-based custom distro). The company currently uses **FreeIPA** for identity management and wants to migrate to **Microsoft Entra ID**.

## Architecture

In this lab, you work with:
- An on-premises-style **Hyper-V host** running Linux virtual machines.
- An **Azure Migrate project + appliance** used to discover servers and workloads and generate assessments.
- A **PaaS target** for PostgreSQL using **Azure Database for PostgreSQL Flexible Server** (private access).
- An **IaaS target** using **Azure VM migration** (Azure Migrate Server Migration).
- Post-migration operations controls (backup, patching, security posture, monitoring, and cost management).

## Exercises

This lab includes the following exercises:

- **Exercise 00**: Prepare for workload migration with Azure Migrate and discover workloads on Hyper-V host (**25 minutes**)
- **Exercise 01**: Assess on-prem workload readiness for migration (**45 minutes**)
- **Exercise 02**: Migrate PostgreSQL to Azure Database for PostgreSQL Flexible Server (**50 minutes**)
- **Exercise 03**: Migrate Linux middleware/runtime server using Azure Migrate (**75 minutes**)
- **Exercise 04**: Governance, security, and cost optimization (**30 minutes**)
- **Exercise 05**: Modernize a legacy app for AKS Automatic with GitHub Copilot


## Prerequisites

- Basic familiarity with the **Azure portal** (resource groups, search, blades).
- Comfort using a browser-based lab environment and switching between tabs/windows.
- Basic Linux navigation concepts (you'll use provided commands and credentials).
- Basic understanding of migration concepts:
  - Discovery and assessment
  - Cutover and validation
  - Rollback and operational readiness