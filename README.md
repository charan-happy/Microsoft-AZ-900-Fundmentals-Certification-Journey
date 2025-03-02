# Microsoft-AZ-900-Fundmentals-Certification-Journey

**Exam Attempted** : 27/2/2025 **Results** : PASS

[My Results](https://learn.microsoft.com/api/credentials/share/en-us/GudiyathamNagacharan-9798/C042E62CFA3BDC1A?sharingId=75E5B4FCD5699429)

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

## Azure Identity, Access, and Security
- Azure Directory services: Microsoft Entra ID is a directory service that enables you to sign in and access both Microsoft cloud applications and cloud applications that you develop. Microsoft Entra ID can also help you maintain your on-premises Active Directory deployment.
  - For on-premises environments, Active Directory running on Windows Server provides an identity and access management service that's managed by your organization. Microsoft Entra ID is Microsoft's cloud-based identity and access management service.
  - With Microsoft Entra ID, you control the identity accounts, but Microsoft ensures that the service is available globally.
  - When you secure identities on-premises with Active Directory, Microsoft doesn't monitor sign-in attempts. When you connect Active Directory with Microsoft Entra ID, Microsoft can help protect you by detecting suspicious sign-in attempts at no extra cost.
  - Microsoft Entra ID can be used by IT administrators, app developers, users, and online service subscribers.
  - Microsoft Entra ID provides services such as authentication, single sign-on, application management, and device management.
  - We can connect on-premises AD with Microsoft Entra ID using Microsoft Entra Connect. Microsoft Entra Connect synchronizes user identities between on-premises Active Directory and Microsoft Entra ID. Microsoft Entra Connect synchronizes changes between both identity systems, so you can use features like SSO, multifactor authentication, and self-service password reset under both systems.

### Microsoft Entra Domain Service
- It is a service that provides managed domain services such as domain join, group policy, lightweight directory access protocol (LDAP), and Kerberos/NTLM authentication.
- Just like Entra ID lets you use directory services without having to maintain the infrastructure supporting it, with Microsoft Entra Domain Services, you get the benefit of domain services without the need to deploy, manage, and patch domain controllers (DCs) in the cloud.
- Microsoft Entra Domain Services managed domain lets you run legacy applications in the cloud that can't use modern authentication methods, or where you don't want directory lookups to always go back to on-premises AD DS environment.
- You can lift and shift those legacy applications from your on-premises environment into a managed domain, without needing to manage the AD DS environment in the cloud.
- Microsoft Entra Domain Services integrates with your existing Microsoft Entra tenant. This integration lets users sign into services and applications connected to the managed domain using their existing credentials. You can also use existing groups and user accounts to secure access to resources.

### How does Microsoft Entra Domain Service work
- When you create Microsoft Entra Domain Services managed domain, you define a unique namespace. This namespace is the domain name. Two Windows Server domain controllers are then deployed into your selected Azure region. This deployment of DCs is known as a replica set.
- We don't need to manage, configure, or update these DCs. The Azure platform handles the DCs as part of the managed domain, including backups and encryption at rest using Azure Disk Encryption.
- A managed domain is configured to perform a one-way synchronization from Microsoft Entra ID to Microsoft Entra Domain Services. You can create resources directly in the managed domain, but they aren't synchronized back to Microsoft Entra ID.
- In a hybrid environment with on-premises AD DS environment, Microsoft Entra Connect synchronizes identity information with Microsoft Entra ID, which is then synchronized to the managed domain.

### Azure Authentication Methods
- Authentication is the process of establishing the identity of a person, service, or device. It requires the person, service, or device to provide some type of credentials to prove who they are.
- Azure supports multiple authentication methods, including standard passwords, single sign-on (SSO), multifactor authentication (MFA), and passwordless.

  - Single sign-on (SSO) enables a user to sign in one time and use that credential to access multiple resources and applications from different providers. For SSO to work, the different applications and providers must trust the initial authenticator. Single sign-on is only as secure as the initial authenticator because the subsequent connections are all based on the security of the initial authenticator.
  - Multifactor authentication is the process of prompting a user for an extra form of identification during the sign-in process. MFA helps protect against a password compromise in situations where the password was compromised but the second factor wasn't.
  - Multifactor authentication increases identity security by limiting the impact of credential exposure.
  - Microsoft Entra multifactor authentication is a Microsoft service that provides multifactor authentication capabilities. Microsoft Entra multifactor authentication enables users to choose an additional form of authentication during sign-in such as a phone call or mobile app notification.
  - Passwordless authentication methods are more convenient because the password is removed and replaced with something you have, plus something you are or something you know. Passwordless authentication needs to be set up on a device before it can work. Each organization has different needs when it comes to authentication. Microsoft global Azure and Azure Government offer the following three passwordless authentication options that integrate with Microsoft Entra ID:
    - Windows Hello for Business
    - Microsoft Authenticator app
    - FIDO2 security keys

- An external identity is a person, device, or service, etc. that is outside your organization. Microsoft Entra ID refers to all the ways you can securely interact with users outside of your organization. If you want to collaborate with partners, distributors, suppliers, or vendors you can share your resources and define how your internal users can access external organizations.
  - With external identities, external users can "bring their own identities" whether they are corporate or government-issued digital identity, or an unmanaged social identity like Google or Facebook they use their own credentials to sign in.

- Conditional access is a tool that Microsoft Entra ID uses to allow (or deny) access to resources based on identity signals. These signals include who the user is, where the user is, and what device the user is requesting access from. Conditional access helps IT administrators: empower users to be productive wherever and whenever, protect the organization's assets. During sign-in, conditional access collects signals from the user, makes decisions based on those signals, and then enforces that decision by allowing or denying the access request or challenging for a multifactor authentication response. Conditional access is useful when you need to: require MFA, require access to services only through approved client applications, require access to your application only from managed devices, block access from untrusted sources.

- Role-based access control is applied to a scope, which is a resource or set of resources that this access applies to. Scope includes: a management group (a collection of multiple subscriptions), a single subscription, a resource group, a single resource. Azure RBAC is hierarchical, in that when you grant access at a present scope, those permissions are inherited by all child processes. Azure RBAC is enforced on any action that's initiated against an Azure resource that passes through Azure Resource Manager. Resource Manager is a management service that provides a way to organize and secure your cloud resources. Azure RBAC doesn't enforce access permissions at the application or data level. Application security must be handled by your application.

- Zero trust is a security model that assumes the worst-case scenario and protects resources with that expectation. Zero trust assumes breach at the outset, and then verifies each request as though it originated from an uncontrolled network. To address this new world of computing, Microsoft highly recommends the zero trust security model, which is based on these guiding principles: verify explicitly, use least privilege access, assume breach. Instead of assuming that a device is safe because it's within the corporate network, it requires everyone to authenticate, then grants access based on authentication rather than location.

- The objective of defense-in-depth is to protect information and prevent it from being stolen by those who aren't authorized to access it.
- Defender for Cloud is a monitoring tool for security posture management and threat protection. It monitors your cloud, on-premises, hybrid, and multicloud environments to provide guidance and notifications aimed at strengthening your security posture.
- When necessary, Defender for Cloud can automatically deploy a Log Analytics agent to gather security-related data. For Azure machines, deployment is handled directly. For hybrid and multicloud environments, Microsoft Defender plans are extended to non-Azure machines with the help of Azure Arc. Cloud security posture management (CSPM) features are extended to multicloud machines without the need for any agents.

## Tools to Manage Azure Environment
- Azure portal (Azure CloudShell)
- Azure PowerShell
- Azure Command Line Interface (CLI) [it is same as PowerShell but difference is that it uses bash commands]

## Additional Tools and Services
- Azure Arc simplifies governance and management by delivering a consistent multi-cloud and on-premises management platform.

### Azure Resource Manager (ARM)
- Azure Resource Manager (ARM) is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account. Anytime you do anything with your Azure resources, ARM is involved.
  - Resource manager template is a JSON file that defines what you want to deploy to Azure.

### ARM Templates
- We can declare the resources that we want in declarative JSON format. The template orchestrates the creation of those resources in parallel. Templates can even execute PowerShell and bash scripts before or after the resource has been set up.
  - ARM Templates provide benefits like declarative syntax, repeatable results, orchestration, modular files, and extensibility.

### Bicep
- Bicep is a language that uses declarative syntax to deploy Azure resources. A Bicep file defines the infrastructure and configuration. Then, ARM deploys that environment based on your Bicep file. Bicep is similar to ARM templates, it tends to use a simpler, more concise style.
  - Some of the benefits of Bicep are: support for all resource types and API versions, simpler syntax, repeatable results, orchestration, and modularity.

- Give it one more read on Azure for governance and policy.

### Azure Advisor
- Evaluates your Azure resources and makes recommendations to help improve reliability, security, and performance, achieve operational excellence, and reduce costs.
- Azure Advisor is designed to help you save time on cloud optimization. The recommendation service includes suggested actions you can take right away, postpone, or dismiss.
- The recommendations are available via the Azure portal and the API, and you can set up notifications to alert you to new recommendations.
- The recommendations are divided into 5 categories: Reliability, Security, Performance, Operational Excellence, and Cost.
- When we are in Azure portal, Advisor dashboard displays personalized recommendations for all your subscriptions.

### Azure Service Health
- Helps you keep track of Azure resources, both your specifically deployed resources and the overall status of Azure. Azure Service Health does this by combining three different Azure services:
  - Azure Status: It is a broad picture of the status of Azure globally.
  - Service Health: It provides a narrower view of Azure services and regions.
  - Resource Health: It is a tailored view of your actual Azure resources. It provides information about the health of individual cloud resources.
  - In the event that a workload you're running is impacted by an event, Azure Service Health provides links to support.

### Azure Monitor
- A platform for collecting data on your resources, analyzing that data, visualizing the information, and even acting on the results.
- Azure Monitor can monitor Azure resources, your on-premises resources, and even multi-cloud resources like virtual machines hosted with a different cloud provider.
- We can use data to help you react to critical events in real-time, through alerts delivered to teams via SMS, email, and so on. Or you can use thresholds to trigger autoscaling functionality to scale to meet the demand.

### Azure Log Analytics
- It is a tool in the Azure portal, where you'll write and run log queries on the data gathered by Azure Monitor. Log Analytics is a robust tool that supports both simple, complex queries, and data analytics. Log Analytics supports both simple, complex queries, and data analysis.

### Azure Monitor Alerts
- An automated way to stay informed when Azure Monitor detects a threshold being crossed.

### Application Insights
- Application Insights, an Azure Monitor feature, monitors your web application. Application Insights is capable of monitoring applications that are running in Azure, on-premises, or in a different cloud environment.
- There are 2 ways to configure Application Insights to help monitor your application. You can either install an SDK in your application or you can use the Application Insights agent. The agent is supported in C#.NET, VB.NET, Java, JavaScript, Node.js, and Python.
- Application Insights not only helps you monitor the performance of your application, but you can also configure it to periodically send synthetic requests to your application, allowing you to check the status and monitor your application even during periods of low activity.


Note : It is just some part of my preparation, if you follow just this repo content for sure you will not able to pass the exam. Other references i used for my preparation are :

- FYI : i didn't completed single resource completely. I studied in all of them though

1. [Microsoft learn (if you read 2 times with understanding More than enough to clear the exam )](https://learn.microsoft.com/en-us/training/azure/)
2. [Freecodecamp course by andrew brown on youtube](https://youtu.be/5abffC-K40c?si=W8LPLzLSjSYRT8d3)
3. [Exam Topics](https://www.examtopics.com/exams/microsoft/az-900/)
