# Before Hands-on Lab Deployment Scripts

This folder contains the Before Hands-on Lab setup deployment scripts for creating the required Azure Resources for this lab.

Select the button below to deploy the existing Tailspin Toys resources for the Hands-on Lab (HOL) to your Azure Subscription:

[![Deploy To Azure](../../images/deploytoazure.svg "Deploy To Azure")](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmicrosoft%2FTechExcel-Securely-migrate-Windows-Server-and-SQL-Server-workloads-to-Azure%2Fmain%2FHands-on%2520lab%2Fresources%2Fdeployment%2Fdeploy.json)
[![Deploy To Azure US Gov](../../images/deploytoazuregov.svg "Deploy to Azure Gov")](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmicrosoft%2FTechExcel-Securely-migrate-Windows-Server-and-SQL-Server-workloads-to-Azure%2Fmain%2FHands-on%2520lab%2Fresources%2Fdeployment%2Fdeploy_gov.json)

The following resources will be provisioned:

- Azure Virtual Networks with VNet Peering
  - Hub and spoke network in Azure
  - Simulated on-premises network in Azure
- Simulated on-premises environment
  - Azure Virtual Machine with Hyper-V hosting a simulated on-premises Windows server machine
  - Azure Virtual Machine hosting SQL Server to simulate an on-premises SQL database server
- Azure Bastion to enable secure Remote Desktop connections to Virtual Machines

## Notes

- This folder contains both an ARM Template (`deploy.json`) file and Azure Bicep (`deploy.bicep`) file for automating the deployment of the Before the Hands-on Lab (HOL) resources necessary for the Hands-on lab.

- When authoring these scripts the infrastructure deployment was authored in Azure Bicep first within the `deploy.bicep` file, and then the Azure Bicep CLI `./bicep build` command was used to build the matching ARM Template.
