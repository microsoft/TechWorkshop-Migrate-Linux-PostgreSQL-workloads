---
title: 'Exercise 04: Governance, security and cost optimization'
layout: default
nav_order: 6
has_children: true
---
# Exercise 04: Governance, security and cost optimization

## Exercise introduction
After migrating the Airsonic application tiers to Azure (Airsonic-Frontend as an Azure VM and the PostgreSQL database on Azure Database for PostgreSQL Flexible Server), you must shift from "migration complete" to "production-ready operations." In this exercise you apply governance and operations controls that organizations typically require before workloads are considered steady-state: backups, patching, security posture management, monitoring dashboards, and cost optimization. You'll also capture a rollback/DR plan to ensure the workload can be recovered quickly if issues arise.

## Exercise description
You'll:
- Protect the migrated VM with Azure Backup.
- Configure Update Manager for ongoing patch assessment and scheduled updates.
- Enable Microsoft Defender for Cloud plans and review recommendations.
- Create a Workbook that visualizes VM performance metrics.
- Review costs and optimization recommendations using Cost Management and Advisor.

## Exercise success criteria
By the end of this exercise, you can demonstrate that:
- The **Airsonic-Frontend** VM is protected by **Azure Backup** and at least one **on-demand backup job** has been triggered.
- **Update Manager** periodic assessment is enabled and a **maintenance configuration** exists for scheduled updates (or you have documented the required prerequisite fix if patch orchestration errors occur).
- **Defender for Cloud** plans for **CSPM, Servers, and Databases** are enabled and you have reviewed at least **one recommendation**.
- A **Monitor Workbook** exists and displays **CPU** and **network traffic** metrics for the Airsonic-Frontend VM over the last 24 hours.
- You have reviewed **costs** for the resource group and captured at least **one Advisor recommendation** (and what you would do with it).
- You have a written **rollback + DR strategy** for both the VM and the database service.

## Expected duration: 30 Minutes