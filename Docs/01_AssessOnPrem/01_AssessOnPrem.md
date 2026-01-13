---
title: 'Exercise 01: Assess On-Prem workload readiness for migration'
layout: default
nav_order: 3
has_children: true
---

# Exercise 01: Assess On-Prem workload readiness for migration

## Introduction
This exercise turns discovery data into actionable migration planning outputs. You'll generate a business case to estimate projected costs and savings, and review the assessment created automatically from that business case to understand readiness and migration recommendations. You'll also define an application for the Airsonic stack so you can reason about the system as a single unit (frontend + backend + workloads), compare PaaS vs IaaS paths, and build a wave plan that sequences migration work. Finally, you'll perform identity planning by mapping FreeIPA identities to Microsoft Entra ID targets to support secure administration and application access after migration.

## Description
In this exercise, you'll:
- Build a business case scoped to the lab environment and review its outputs (scope, cost comparison, savings, and strategy summaries).
- Explore discovered inventory to confirm servers and workloads were detected (Airsonic web app and PostgreSQL database).
- Define an application for the Airsonic stack by linking the frontend and backend servers and their discovered workloads.
- Review the assessment created by the business case and compare modernization options (PaaS preferred, PaaS only, lift-and-shift to Azure VMs).
- Create a wave plan from the recommended path, add tasks, review selected applications/workloads, and inspect target settings and migration options.
- Document a planning-only identity mapping strategy from FreeIPA to Microsoft Entra ID, including admins, users, and service identities.

## Success criteria
- A business case named **bc-@lab.LabInstance.Id** exists and reflects the expected scope (workloads/web apps/databases).
- The assessment **businesscase-bc-@lab.LabInstance.Id** is accessible, shows the expected workload count, and provides clear path comparisons across PaaS and IaaS options.
- An application named **airsonic-app-@lab.LabInstance.Id** exists and includes the linked servers and discovered workloads.
- A wave plan named **wave-@lab.LabInstance.Id** exists and includes the Airsonic application and expected workloads, with tasks and target settings reviewed.
- A FreeIPA-to-Entra identity mapping table is completed with at least six entries covering admin, user, and service identities.

## Key tasks
- Generate a business case and interpret its cost/savings outputs while validating the scope matches discovered inventory.
- Create an application definition for the Airsonic stack so planning reflects an application boundary rather than individual servers.
- Use the assessment to compare PaaS vs IaaS paths and identify recommended targets for the web app and PostgreSQL database.
- Create a wave plan from the recommended path, add migration tasks, and review workload selection and target settings.
- Document a practical identity mapping strategy from FreeIPA to Entra ID to support post-migration administration and access control.

## Expected duration: 45 Minutes
