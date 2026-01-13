---
title: 'Exercise 02: Migrate PostgreSQL to Azure Database for PostgreSQL Flexible Server'
layout: default
nav_order: 4
has_children: true
---

# Exercise 02: Migrate PostgreSQL to Azure Database for PostgreSQL Flexible Server

## Introduction
This exercise modernizes the database tier by migrating the on-premises PostgreSQL backend to Azure Database for PostgreSQL Flexible Server using private access. You'll deploy the flexible server, ensure the lab environment has the required hybrid connectivity, validate migration readiness, perform the migration, and then verify the application successfully uses the new database target. The goal is to reinforce modernization benefits (managed platform service) while practicing validation, cutover, and post-migration functional checks.

## Description
In this exercise, you'll:
- Deploy a PostgreSQL flexible server with private access (VNet integration), specifying compute, authentication, and networking settings.
- Establish/confirm hybrid connectivity (VPN) required to reach private Azure endpoints from the lab environment.
- Create a simple pre-migration marker inside the Airsonic application and confirm the current on-prem database endpoint.
- Retrieve the flexible server's internal IP address from Private DNS records for later connectivity configuration and validation.
- Run a validation migration, review results, then run an offline migration of the Airsonic database to flexible server.
- Update the application configuration to point to the migrated database and verify application behavior and data after cutover.

## Success criteria
- A PostgreSQL flexible server named **pgsql-flex-@lab.LabInstance.Id** is deployed successfully using private access.
- Hybrid connectivity is active so the lab environment can reach the flexible server via private networking/DNS.
- Database migration validation completes successfully and the migration job completes with status **Succeeded**.
- The Airsonic application is configured to use the new database target and the pre-migration marker (playlist) is still present after migration.
- Database settings reflect the new target endpoint after cutover verification.

## Key tasks
- Deploy PostgreSQL flexible server using private access and confirm it is reachable through the lab's hybrid connectivity.
- Establish a pre-migration validation marker and confirm the application's original database endpoint.
- Retrieve the flexible server private IP via Private DNS to support configuration and troubleshooting.
- Validate and migrate the PostgreSQL database using the Azure Database Migration Service workflow.
- Update application connectivity to the migrated database and verify application function and data integrity.

## Expected duration: 50 Minutes