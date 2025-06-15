# Managing Storage

# PPT - Storage Overview

# PPT - Azure Storge Accounts
- Enterprise Cloud Storage
- Deployed as an Azure resource

# PPT Storage Account Contents
- Binary large objects (blobs)
- File shares
- Queues
- Tables

# PPT Storage Account Settings
- Access Keys
- Shared Access Signatures (SAS)
- Encryption
- Geo-replication

# Storage Account Blobs
- File (blob) storage
- Blobs are organized within blob containers
- Blob settings:
  - Hot, Cool, and Archive storage tiers
  - Automated life cycle management
  - Blob public access
  - Versioning, snapshots
  - Soft delete

# PPT Blob Types
- Blobs are files
- Block ( smaller types of files )
- Page (virtual disks used by virtual machines)
- Append (normally used when you are writing to an end of a file, such as a case with log files)

# PPT Storage Account File Shares
- Shared folder access from on--premises or in the cloud over Transmission Control Protocol (TCP) port 445
- OS must support at least Server Message Block (SMB) v3.0
- Accessible via drive mappings and mount points.

# PPT Storage Account Queues
- Storage Account Queues would be of interest to software developers.
- Support there is an application, and this application has multiple components which need to communicate with each other via messages.
- Suppose there is a component 'component # 1' and second component 'component # 2', and both components are running fine.
- App component # 1 can drop messages in the queue storage account, and App component # 2 can read that message and process it.
- So, it's a centralized storage solution for inter-application component messaging.
- 
