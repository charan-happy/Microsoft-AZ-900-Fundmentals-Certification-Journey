# Microsoft-AZ-900-Fundmentals-Certification-Journey

 # Microsoft Azure 900 Syllabus

## Describe Cloud Concepts (20-25%)
- Introduction to cloud computing
- What is cloud computing
- Describe a shared responsibility model
- Define cloud models
- Describe the consumption-based model
- Describe cloud service types (IAAS, PAAS, SAAS)

## Describe Core Azure Services (15-20%)
- What is Microsoft Azure
- Get started with Azure accounts
- Describe Azure physical infrastructure
- Describe Azure Management infrastructure

### Describe Azure Compute and Networking Services
- Describe Azure virtual machines
- Describe Azure virtual desktop
- Describe Azure containers
- Describe Azure functions
- Describe application hosting options
- Describe Azure virtual networking
- Describe Azure private networks
- Describe Azure ExpressRoute
- Describe Azure DNS

### Describe Azure Storage Services
- Describe Azure storage accounts
- Describe Azure storage redundancy
- Describe Azure storage services
- Describe Azure data migration options

### Describe Azure Identity, Access, and Security
- Describe Azure directory services
- Describe Azure authentication methods
- Describe Azure external identities
- Describe Azure conditional access
- Describe Azure role-based access control
- Describe zero trust model
- Describe defense-in-depth
- Describe Microsoft Defender for Cloud

## Describe Core Solutions and Management Tools on Azure (10-15%)
- Describe cost management in Azure
  - Describe factors that can affect costs in Azure
  - Compare the pricing and total cost of ownership calculators
  - Describe Microsoft cost management tool
  - Describe purpose of tags
- Describe features and tools in Azure for governance and compliance
  - Describe the purpose of Microsoft Purview
  - Describe the purpose of Azure Policy
  - Describe the purpose of resource locks
  - Describe the purpose of the Service Trust Portal
- Describe the features and tools for managing and deploying Azure resources
  - Describe tools for interacting with Azure
  - Describe the purpose of Azure Arc
  - Describe Azure Resource Manager and Azure ARM templates
- Describe monitoring tools in Azure
  - Describe the purpose of Azure Advisor
  - Describe the Azure Service Health
  - Describe Azure Monitor

## Tools to Manage Azure Environment
- Azure portal (Azure CloudShell)
- Azure PowerShell
- Azure Command Line Interface (CLI) [it is same as PowerShell but difference is that it uses bash commands]

## Additional Tools and Services
- Azure Arc simplifies governance and management by delivering a consistent multi-cloud and on-premises management platform.

### Azure Advisor
- Evaluates your Azure resources and makes recommendations to help improve reliability, security, and performance, achieve operational excellence, and reduce costs.
- Designed to help you save time on cloud optimization. The recommendation service includes suggested actions you can take right away, postpone, or dismiss.
- Recommendations are available via the Azure portal and the API, and you can set up notifications to alert you to new recommendations.
- Recommendations are divided into 5 categories: Reliability, Security, Performance, Operational Excellence, and Cost.
- When in Azure portal, Advisor dashboard displays personalized recommendations for all your subscriptions.

### Azure Service Health
- Helps you keep track of Azure resources, both your specifically deployed resources and the overall status of Azure. Azure Service Health does this by combining three different Azure services:
  - Azure Status: It is a broad picture of the status of Azure globally.
  - Service Health: It provides a narrower view of Azure services and regions.
  - Resource Health: It is a tailored view of your actual Azure resources. It provides information about the health of individual cloud resources.
  - In the event that a workload you're running is impacted by an event, Azure Service Health provides links to support.

### Azure Monitor
- A platform for collecting data on your resources, analyzing that data, visualizing the information, and even acting on the results.
- Can monitor Azure resources, your on-premises resources, and even multi-cloud resources like virtual machines hosted with a different cloud provider.
- Use data to help you react to critical events in real-time, through alerts delivered to teams via SMS, email, and so on. Or you can use thresholds to trigger autoscaling functionality to scale to meet the demand.

### Azure Log Analytics
- A tool in the Azure portal, where you'll write and run log queries on the data gathered by Azure Monitor. Log Analytics is a robust tool that supports both simple, complex queries, and data analytics.

### Azure Monitor Alerts
- An automated way to stay informed when Azure Monitor detects a threshold being crossed.

### Application Insights
- An Azure Monitor feature, monitors your web application. Application Insights is capable of monitoring applications that are running in Azure, on-premises, or in a different cloud environment.
- There are 2 ways to configure Application Insights to help monitor your application. You can either install an SDK in your application or you can use the Application Insights agent. The agent is supported in C#.NET, VB.NET, Java, JavaScript, Node.js, and Python.
- Application Insights not only helps you monitor the performance of your application, but you can also configure it to periodically send synthetic requests to your application, allowing you to check the status and monitor your application even during periods of low activity.
