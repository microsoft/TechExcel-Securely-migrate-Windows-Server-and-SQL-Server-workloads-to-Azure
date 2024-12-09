---
title: 'Exercise 00: Lab Setup'
layout: default
nav_order: 2
has_children: true
---

# Exercise 00 - Lab Setup

## Lab Scenario

In this lab, attendees will perform steps toward migrating Tailspin Toy's on-premises Windows Server and SQL Server workloads to Azure. Tailspin needs a new Windows Server VM created in Azure for hosting their Web application, an on-premises SQL Server database migrated to Azure SQL Managed Instance, secure Windows Server, and an on-premises Windows Server VM to be Azure Arc-enabled.
Tailspin already has a Hub and Spoke network setup in Azure with Azure Bastion for enabling secure remote management of Azure VM using Azure Bastion. The Azure resources provisioned throughout this lab will be deployed into this environment.

In this first exercise, you will retrieve the ID for your Entra ID user account, as well as deploy the resources needed to simulate the on-prem environment of Tailspin Toy's.

## Objectives

After you complete this exercise, you will be able to:

* Find an Entra ID user ID
* Validate Resource providers
* Deploy an ARM Template

## Lab Duration

* **Estimated Time:** 180 minutes
