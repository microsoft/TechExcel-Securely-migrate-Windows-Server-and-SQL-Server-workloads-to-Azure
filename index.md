---
title: Introduction
layout: home
nav_order: 1
---

# TechExcel: Securely migrate Windows Server and SQL Server workloads to Azure

In this lab, attendees will perform steps toward migrating Tailspin Toy's on-premises Windows Server and SQL Server workloads to Azure. Tailspin needs a new Windows Server VM created in Azure for hosting their Web application, an on-premises SQL Server database migrated to Azure SQL Managed Instance, secure Windows Server, and an on-premises Windows Server VM to be Azure Arc-enabled.
Tailspin already has a Hub and Spoke network setup in Azure with Azure Bastion for enabling secure remote management of Azure VM using Azure Bastion. The Azure resources provisioned throughout this lab will be deployed into this environment.

## Solution architecture

![Diagram showing on-premises network connected to Azure using Azure ExpressRoute with a Hub and Spoke network in Azure. The Spoke VNet contains the migrated Front-end, Back-end, and SQL Database workloads running within Subnets inside the Spoke VNet in Azure.](/Hands-on%20lab/images/PreferredSolutionDiagram.png "Preferred Solution Diagram")

The diagram shows an on-premises network connected to Azure using Azure ExpressRoute with a Hub and Spoke network in Azure. The Spoke VNet contains the migrated Front-end, Back-end, and SQL Database workloads running within Subnets inside the Spoke VNet in Azure.

### Redundant Azure ExpressRoute peering locations

Redundant Azure ExpressRoute peering locations provide an additional layer of resiliency and high availability for your connectivity to Azure. With redundant peering locations, you can establish ExpressRoute circuits in two different peering locations, providing a backup connection in case of an outage or disruption in one of the locations.

This redundancy ensures that your connectivity to Azure remains uninterrupted, even in the event of a failure in one of the peering locations. By leveraging redundant peering locations, you can minimize downtime and ensure that your workloads and applications continue to run smoothly, even in the face of unexpected disruptions.

{: .note }
> You can find more information about Redundant Azure ExpressRoute peering locations at [https://learn.microsoft.com/en-us/azure/expressroute/designing-for-disaster-recovery-with-expressroute-privatepeering](https://learn.microsoft.com/en-us/azure/expressroute/designing-for-disaster-recovery-with-expressroute-privatepeering) and [https://azure.microsoft.com/en-us/blog/building-resilient-expressroute-connectivity-for-business-continuity-and-disaster-recovery-2/](https://azure.microsoft.com/en-us/blog/building-resilient-expressroute-connectivity-for-business-continuity-and-disaster-recovery-2/).

### S2S VPN as a backup for ExpressRoute private peering

A Site-to-Site (S2S) VPN connection can be used as a secure failover path for ExpressRoute private peering. This means that if the ExpressRoute connection experiences an outage or disruption, the S2S VPN connection can provide a backup connection to ensure continued connectivity to Azure.

To set up a S2S VPN connection as a backup for ExpressRoute private peering, you need to create two virtual network gateways for the same virtual network: one using the gateway type 'VPN' and the other using the gateway type 'ExpressRoute'. Once the S2S VPN connection is configured, it can provide a secure and reliable failover path for ExpressRoute private peering, ensuring that your connectivity to Azure remains uninterrupted even in the event of an outage or disruption in the ExpressRoute connection. 

{: .note }
> You can find more information about Redundant Azure ExpressRoute peering locations at [https://learn.microsoft.com/en-us/azure/expressroute/use-s2s-vpn-as-backup-for-expressroute-privatepeering](https://learn.microsoft.com/en-us/azure/expressroute/use-s2s-vpn-as-backup-for-expressroute-privatepeering)


### Zone-aware SKUs

Azure zone-aware SKUs provide high availability and resiliency for your workloads and applications by distributing resources across multiple availability zones within an Azure region. Each availability zone is a separate physical location with independent power, cooling, and networking, providing protection against datacenter-level failures.

By using zone-aware SKUs, you can deploy your resources, such as virtual machines, managed disks, and load balancers, across multiple availability zones, ensuring that your workloads and applications remain available even if one of the zones experiences an outage. This redundancy helps to minimize downtime and ensure that your services continue to run smoothly, even in the face of unexpected disruptions.

{: .note }
> You can find more information about Azure Availability Zones at [https://learn.microsoft.com/en-us/azure/reliability/availability-zones-overview?tabs=azure-cli](https://learn.microsoft.com/en-us/azure/reliability/availability-zones-overview?tabs=azure-cli).



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