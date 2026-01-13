---
title: 'Exercise 03: Migrate Linux Middleware/Runtime Server using Azure Migrate'
layout: default
nav_order: 5
has_children: true
---

# Exercise 03: Migrate Linux Middleware/Runtime Server using Azure Migrate

## Introduction
This exercise applies Azure Migrate Server Migration to move a Hyper-V VM to Azure as an Azure VM (lift-and-shift). You'll prepare the Hyper-V replication environment, install and register the replication provider, configure required Azure-side resources and permissions, replicate the VM, perform a planned migration cutover, and then validate that the migrated workload runs successfully in Azure. The focus is on learning the end-to-end mechanics of VM migration using Azure Migrate and understanding what "complete" looks like after cutover (testing + stopping replication).

## Description
In this exercise, you'll:
- Deploy the Azure Migrate replication resources for Hyper-V migrations and download required provider/credential files on the Hyper-V host.
- Install the Hyper-V replication provider and register the Hyper-V host to the Recovery Services vault used by Azure Migrate.
- Finalize registration in the Azure portal and configure required permissions so replication can access the cache storage account.
- Start replication of the target VM using assessment-based settings and monitor until replication reaches a protected state.
- Perform a planned migration (cutover) to create and start the Azure VM using the latest replicated data.
- Stop replication after migration and validate workload/application functionality on the migrated Azure VM.

## Success criteria
- The Hyper-V host is successfully registered and finalized for Azure Migrate Server Migration.
- Replication begins and the VM reaches a **Protected** replication status.
- Planned migration completes successfully and the Azure VM is created and running.
- Replication is stopped after cutover and replication state is cleaned up.
- The migrated workload is validated in Azure (the application is reachable and expected data/behavior is confirmed).

## Key tasks
- Prepare Hyper-V migration prerequisites: provider installation, host registration, and Azure resource readiness.
- Configure required permissions so replication can use the cache storage account successfully.
- Replicate the VM using assessment-derived settings and monitor replication health/status.
- Execute a planned migration cutover and validate the migrated VM in Azure.
- Finalize migration by stopping replication and confirming the workload operates as expected post-migration.

## Expected duration: 75 Minutes