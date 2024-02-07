# Tech Excel: Securely migrate Windows Server and SQL Server workloads to Azure

Tailspin Toys is a global manufacturer of children’s toys that was founded in 1957 with its global headquarters located in Milwaukee, WI. Their mission-critical workloads are currently hosted in an on-premises datacenter and are beginning a journey to modernize and migrate into the cloud using Microsoft Azure.

During the Envision Workshop, Kaylee Frye, CTO of Tailspin Toys, saw the value of digital transformation, adopting the Microsoft Azure cloud, and modernizing their infrastructure. She has already had the Technical Architects at Tailspin Toys begin assessing their current environment and what it will take to migrate to the cloud. They are looking to optimize their technology investments by reducing technical debt, streamlining operations, and simplifying their DevOps workflow. According to Kaylee Frye, "Our development teams have already begun adopting DevOps strategies and implemented CI/CD (continuous integration and continuous delivery) pipelines with Azure DevOps. We really look forward to better streamlining IT operations as we adopt Microsoft Azure for the infrastructure too."


## Target audience

- Enterprise Architects
- Infrastructure Engineers

## Abstracts

### Workshop

In this workshop, you will gain experience designing and implementing a strategy for securely migrating Windows Server and SQL Server workloads to Azure, and enabling on-premises virtual machines management by using Azure Arc.

At the end of the workshop, you will be better able to design and implement an Azure migration strategy for Windows Server and SQL Server workloads using Azure Virtual Machines, Azure SQL Managed Instance (SQL MI), and Azure Arc.


### Hands-on Lab

In this lab, attendees will perform steps toward migrating Tailspin Toy's on-premises Windows Server and SQL Server workloads to Azure. Tailspin needs a new Windows Server VM created in Azure for hosting their Web application, an on-premises SQL Server database migrated to Azure SQL Managed Instance, and an on-premises Windows Server VM to be Azure Arc-enabled.

Tailspin already has a Hub and Spoke network setup in Azure with Azure Bastion for enabling remote management of Azure VM using Azure Bastion. The Azure resources provisioned throughout this lab will be deployed into this environment.

At the end of this hands-on lab, you will be better able to set up a Windows Server for application migration to Azure, migrate an on-premises SQL Database to Azure SQL Managed Instance, and Azure Arc-enable an on-premises virtual machine so it can be managed from Azure.

Continue to the [Hands-on lab](Hands-on%20lab) documents folder.

## Azure services and related products

- Azure VMs
- Azure Arc
- Azure SQL Managed Instance
- Azure Networking
- Microsoft Data Migration Assistant
- Azure Data Studio - Azure SQL Migration Extension

## Azure solutions

DC Migration

## Related references
- [Microsoft Defender for Cloud](https://learn.microsoft.com/en-us/azure/defender-for-cloud/)
- [Azure Arc](https://docs.microsoft.com/azure/azure-arc/overview)
- [Azure SQL Managed Instance](https://docs.microsoft.com/en-us/azure/azure-sql/managed-instance/sql-managed-instance-paas-overview)



## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
