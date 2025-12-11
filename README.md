# Azure Storage Lab – Full Walkthrough

This repo documents my full hands-on walkthrough of Azure Storage services as completed in the Microsoft Ignite Skills Challenge. I deployed a Storage Account, explored Blob Storage, enabled ADLS Gen2, created File Shares, and worked with Azure Table Storage. Every step was completed inside the Azure Portal.

---

## Overview

This project demonstrates practical, real-world use of Azure Storage capabilities. I created and configured a Storage Account, uploaded JSON files, enabled hierarchical namespaces, created folders and directories, mounted file shares, and inserted entities into Azure Tables. Screenshots show evidence of every action.

---

## What This Repo Includes
- Storage Account creation  
- Blob Storage + container structure  
- JSON file uploads  
- ADLS Gen2 hierarchical namespace exploration  
- Azure File Share creation  
- Azure Table Storage creation + entity insertion  
- Screenshot evidence of each stage  

---

## Repo Structure
---

## Skills Demonstrated
- Azure Storage configuration  
- Blob containers + virtual directories  
- File uploads and metadata  
- ADLS Gen2 directory + ACL model  
- File Share provisioning  
- Table Storage entities  
- Portal navigation + resource management  

---

# Full Implementation Steps

## 1. Provision Azure Storage Account
- Created a Storage Account with Standard performance and LRS redundancy.  
- Reviewed advanced options and noted where hierarchical namespace can be enabled.  
- Disabled soft delete options temporarily to follow lab instructions and avoid conflicts.  
- Validated configuration and deployed the resource.

---

## 2. Explore Blob Storage
- Opened Containers under the storage account.  
- Created a container named *data* with private access.  
- Used Storage Browser to confirm folder and blob structure.  
- Created a virtual folder using “Add Directory” to observe flat namespace behavior.

---

## 3. Upload JSON Files
- Downloaded product1.json.  
- Uploaded it into the blob container under a virtual folder named *product_data*.  
- Noted that folders appear only when blobs exist (flat namespace behavior).

---

## 4. Enable ADLS Gen2 (Hierarchical Namespace)
- Enabled hierarchical namespace via the Data Lake Gen2 upgrade page.  
- Verified that pre-existing folders and blobs remained accessible.  
- Uploaded product2.json to confirm new hierarchical behavior.  
- Reviewed new folder-level options like rename and permissions.

---

## 5. Explore Azure File Shares
- Created a file share named *files* using the Transaction Optimized tier.  
- Disabled backup to reduce cost.  
- Opened the Connect panel to view SMB/NFS mount commands for Windows, Linux, and macOS.

---

## 6. Explore Azure Tables
- Created a table named *products*.  
- Inserted first entity:  
  - PartitionKey: 1  
  - RowKey: 1  
  - Name: Widget  
  - Price: 2.99  
- Inserted second entity:  
  - PartitionKey: 1  
  - RowKey: 2  
  - Name: Kniknak  
  - Price: 1.99  
  - Discontinued: true  
- Verified rows and timestamp column.

---

## 7. Cleanup
If no longer needed, the entire resource group can be deleted to avoid charges.

---

## Purpose of This Repo
This repository serves as a learning record, a personal reference for Azure Storage fundamentals, and a portfolio piece showing hands-on cloud administration completed end-to-end.

---
