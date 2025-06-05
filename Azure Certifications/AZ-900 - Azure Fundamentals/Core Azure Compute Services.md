# Core Azure Compute Services and Products

## What is Compute Service
- Remember that not all VM types are available in all regions, so therefore select the VM type and the region carefully. 

## Different Compute Services and Products offered by Azure
- https://learn.microsoft.com/en-us/azure/architecture/guide/technology-choices/compute-decision-tree
- **Azure Virtual Machines:** A service where you deploy and manage virtual machines (VMs) inside an Azure virtual network.
- **Azure App Service:** A managed service for hosting web apps, mobile app back ends, RESTful APIs, or automated business processes.
- **Azure Function:** A service that provides managed functions that run based on a variety of trigger types for event-driven applications.
- **Azure Kubernetes Service (AKS):** A managed Kubernetes service for running containerized applications.
- **Azure Container Apps:** A managed service built on Kubernetes, which simplifies the deployment of containerized applications in a serverless environment.
- **Azure Container Instances:** This service is a fast and simple way to run a single container or group of containers in Azure.
                             Azure Container Instances doesn't provide full container orchestration, but you can implement them without having to provision
                             any VMs or adopt a higher-level service.
- **Azure Red Hat Open Shift:** A fully managed OpenShift cluster for running containers in production with Kubernetes.
- **Azure Service Fabric:** A distributed systems platform that can run in many environments, including Azure or on-premises.
- **Azure Batch:** A managed service for running large-scale parallel and high-performance computing (HPC) applications.
- **Azure VMWare Solution:** A managed service for running VMware workloads natively on Azure.

# Understand different Hosting Models for Compute Services

- Infrastructure-as-a-service (IaaS)
- Platform-as-a-service (PaaS)
- Function-as-a-Service (FaaS)

# Microservices Compute Option
- https://learn.microsoft.com/en-us/azure/architecture/microservices/design/compute-options
- The term compute refers to the hosting model for the computing resources that your application runs on.
- For a microservices architecture, the following approaches are popular:
  - Deploy microservices on dedicated compute platforms, typically by using a microservice orchestrator.
  - Deploy microservices on a serverless platform.
  - Following are teh Microservices compute options and products offered by Azure:
    - Azure Kubernetes Service (AKS)
    - Container Apps
    - Service Fabric
    - Red Hat OpenShift


# Availability
There are multiple options to manage the availability of your virtual machines in Azure

- Availability Zones
    - Availability Zones are physically separated zones within an Azure region.
    - Availability zones guarantee virtual machine connectivity to at least one instance at least 99.99% of the time when you have two or more instances deployed 
      across two or more Availability Zones in the same Azure region.
- Virtual Machine Scale Set
    -  Virtual Machine Scalet Set let you create and manage a group of load balanced virtual machines.
    -  The number of virtual machine instances can automatically increase or decrease in response to demand or a defined schedule.
    -  Scale sets provide high availability to your applications, and allow you to centrally manage, configure, and update many virtual machines.
    -  Virtual machines in a scale set can also be deployed into multiple availability zones, a single availability zone, or regionally.
 
# Sizes and Pricing
- The size of the virtual machine that you use is determined by the workload that you want to run.
- The size that you choose then determines factors such as processing power, memory, storage capacity, and network bandwidth.
- Azure offers a wide variety of sizes to support many types of uses.
- Azure charges an hourly price based on the virtual machine’s size and operating system.
- For partial hours, Azure charges only for the minutes used.
- Storage is priced and charged separately.

  # Managed Disks
  - Managed Disks handles Azure Storage account creation and management in the background for you,
  - and ensures that you don't have to worry about the scalability limits of the storage account.
  - You specify the disk size and the performance tier (Standard or Premium), and Azure creates and manages the disk.
  - As you add disks or scale the virtual machine up and down, you don't have to worry about the storage being used.
  - If you're creating new virtual machines, use the Azure CLI or the Azure portal to create virtual machines with Managed OS and data disks.
  - If you have virtual machines with unmanaged disks, you can convert your virtual machines to be backed with Managed Disks.
  - You can also manage your custom images in one storage account per Azure region,
  - and use them to create hundreds of virtual machines in the same subscription.
  - For more information about Managed Disks, see the Managed Disks Overview.


  - Azure managed disks are block-level storage volumes managed by Azure and used with Azure Virtual Machines.
  - Managed disks are like physical disks in an on-premises server, but they're virtualized.
  - With managed disks, you only have to specify the disk type and the disk size, then provision the disk.
  - After you provision the disk, Azure handles the rest.
 
  - There are five types of managed disks: Ultra Disks, Premium solid-state drives (SSD) v2, Premium SSD, Standard SSD, and Standard hard disk drives (HDD).
  - To learn about each disk type and decide which fits your needs, see Azure managed disk types.
 
  - An alternative is to use Azure Elastic SAN as the storage for your virtual machine (VM). With Elastic SAN, you can consolidate the storage for all your workloads into a single storage back end. Elastic SAN can be more cost effective if you have many large-scale, I/O-intensive workloads and top-tier databases. To learn more, see What is Azure Elastic SAN?.
  # Demo # 1 - Basic Tutorial - How to Create a new Virtual Machine using Azure Portal
  
   

