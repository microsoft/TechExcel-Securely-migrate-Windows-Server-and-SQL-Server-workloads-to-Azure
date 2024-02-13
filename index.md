---
title: Introduction
layout: home
nav_order: 1
---

# TechExcel: Securely migrate Windows Server and SQL Server workloads to Azure

In this lab, attendees will perform steps toward migrating Tailspin Toy's on-premises Windows Server and SQL Server workloads to Azure. Tailspin needs a new Windows Server VM created in Azure for hosting their Web application, an on-premises SQL Server database migrated to Azure SQL Managed Instance, secure Windows Server, and an on-premises Windows Server VM to be Azure Arc-enabled.
Tailspin already has a Hub and Spoke network setup in Azure with Azure Bastion for enabling secure remote management of Azure VM using Azure Bastion. The Azure resources provisioned throughout this lab will be deployed into this environment.


## Exercises

This lab has exercises on:

* Provisioning a Windows Server VM
* Set up a Windows Server for application migration to Azure
* Migrate an on-premises SQL Server Database to Azure SQL Managed Instance (SQL MI)
* Secure Windows Server
* Enable Azure Arc on an on-premises virtual machine so it can be managed from Azure

This lab is available as GitHub pages [here](https://microsoft.github.io/TechExcel-Securely-migrate-Windows-Server-and-SQL-Server-workloads-to-Azure)


## Prerequisites

For running this lab you will need:

* An Azure subscription without a spending cap to deploy the Barracuda firewall from the Azure Marketplace.
* A desktop, laptop, or virtual machine and access to install software on that machine.