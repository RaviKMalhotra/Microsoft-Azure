- As an Azure Administrator, you will need the skills to create and manage storage accounts and blobs.
Begin this course by learning to plan the number, location, and configuration of Azure storage accounts.
Next, you will find out how to create storage accounts and manage blobs using the portal, the command line interface (CLI), AzCopy, Azure Storage Explorer, and PowerShell. Then you will discover how to enable storage account blob features such as soft delete and versioning. Finally, you will examine how to configure immutable blob policies, manage storage tier and archiving, and automate blob life cycle management. This course can be used to prepare for exam AZ-104: Microsoft Azure Administrator.
# Managing Storage


# PPT - Storage Overview

# PPT - Azure Storge Accounts
- Enterprise Cloud Storage
- Deployed as an Azure resource

## PPT Storage Account Contents
- Binary large objects (blobs)
- File shares
- Queues
- Tables

## PPT Storage Account Settings
- Access Keys
- Shared Access Signatures (SAS)
- Encryption
- Geo-replication

## Storage Account Blobs
- File (blob) storage
- Blobs are organized within blob containers
- Blob settings:
  - Hot, Cool, and Archive storage tiers
  - Automated life cycle management
  - Blob public access
  - Versioning, snapshots
  - Soft delete

## PPT Blob Types
- Blobs are files
- Block ( smaller types of files )
- Page (virtual disks used by virtual machines)
- Append (normally used when you are writing to an end of a file, such as a case with log files)

## PPT Storage Account File Shares
- Shared folder access from on--premises or in the cloud over Transmission Control Protocol (TCP) port 445
- OS must support at least Server Message Block (SMB) v3.0
- Accessible via drive mappings and mount points.

## PPT Storage Account Queues
- Storage Account Queues would be of interest to software developers.
- Support there is an application, and this application has multiple components which need to communicate with each other via messages.
- Suppose there is a component 'component # 1' and second component 'component # 2', and both components are running fine.
- App component # 1 can drop messages in the queue storage account, and App component # 2 can read that message and process it.
- So, it's a centralized storage solution for inter-application component messaging.

## PPT Storage Account Tables
- These are NoSQL-based key and value pairs.
- It uses an unstructured schema, unlike a relational database which strictly defines field types, data types, the amount of data that can be put into it, and so on.
- Storage for Key and value pairs (so, this is just a key and value pair basic storage)

# Creating an Azure Storage Account
- Storage account name has to be unique and in lower case letters
- Performance settings - There are 2 performance settings
  - Standard: Recommended for most scenarios (general-purpose v2 account)
  - Premium: Recommended for scenarios that require low latency and it 
- Redundancy options: default setting for redundancy is GRS. 
  - Locally Redundant Storage (LRS) - lowest cost option with basic protection against server rack and drive failures. used for non-critical scenarios
  - Geo-redundant storage - Immediate option with failover capabilities in a secondary region, it is recommended for backup scenarios. It will automatically create a synchronized copy of the storage account in the secondary region, a different region.
  - There are multiple tabs you need to deal with while creating a storage accoutn such as Basics, Advanced, Networking, Data Protection, Encryption, Tags
  - Minimum TLS Version is set to 1.2
  - Default Blob Access tier is set to Hot
  - Hot Blob Access tier is optimized for frequently accessed data and everyday usage scenarios.
  - Cool Access tier is optimized for infrequently accessed data and backup scenarios.
  - There is a price difference between Hot and Cool Access tier.
  - 'Allow cross-tenant replication' option is not selected by default.
  - 'Network Access' default option is set to - Enable public access from all networks. you can change this to other options such as
  - other otions are 'Enable public access from selected virtual networks and IP addresses' and select the desired virtual network.
  - and 'Disable public access and anable private access', and create and select the private endpoint.
  - 
  - 
