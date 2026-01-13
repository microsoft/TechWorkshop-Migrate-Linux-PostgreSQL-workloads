---
title: 'Exercise 00: Prepare for workload migration with Azure Migrate and discover workloads on Hyper-V Host'
layout: default
nav_order: 2
has_children: true
---

# Exercise 00: Prepare for workload migration with Azure Migrate and discover workloads on Hyper-V Host

## Introduction
This exercise establishes the Azure Migrate foundation for the lab. You'll create a dedicated Azure Migrate project and register the Azure Migrate appliance that is pre-deployed in the lab environment. With the project and appliance connected, you'll configure discovery against the Hyper-V host and enable guest/workload discovery so Azure Migrate can detect both server inventory and workload-level objects such as the Airsonic web app (Tomcat) and PostgreSQL database. The outputs of this exercise become the source data for later business case creation, assessments, and migrations.

## Description
In this exercise, you'll:
- Sign in to the Azure portal and create a new Azure Migrate project in the provided subscription and resource group.
- Initiate Hyper-V appliance-based discovery, generate a project key, and register the Azure Migrate appliance using device sign in.
- Configure discovery credentials for the Hyper-V host and guest workloads (Linux and PostgreSQL).
- Add the Hyper-V host as a discovery source, validate connectivity, and start discovery so the project begins collecting inventory and workload information.

## Success criteria
- A new Azure Migrate project named **Migration-Project-@lab.LabInstance.Id** exists and can be opened successfully.
- The Azure Migrate appliance is registered to the project and shows a successful/healthy registration status.
- The Hyper-V host discovery source validates successfully and discovery is started.
- Azure Migrate begins populating discovered inventory with the expected servers and workload objects (including a detected web app and PostgreSQL workload).

## Key tasks
- Create and open an Azure Migrate project that will serve as the workspace for discovery, assessment, and migration activities.
- Generate a project key and register the pre-deployed Azure Migrate appliance to the project using device sign in.
- Configure Hyper-V discovery and guest discovery credentials (Linux + PostgreSQL) to enable workload identification.
- Add the Hyper-V host as a discovery source, validate access, and start discovery to populate inventory and workloads.

## Expected duration: 25 Minutes