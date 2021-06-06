# Notes for AZ-900: Microsoft Azure Fundamentals exam: level 1
## 1. Cloud concepts

## 2. Azure Architecture

## 3. Computing
### Virtual Machine (VM)
Digital version of hardware that you control exclusively. You pay for VMs hourly.

### Scale Sets
Set of multiple VMs that can be added or removed.

### App Services
A managed platform to host web applications (PaaS)

### Azure Container Instances 
Runs containers on Azure

### Azure Kubernetes Service
Service to ease work on many containers.

### Windows Virtual Desktop
Use Windows 10 anywhere.

### Functions
Piece of code that does one task without maintaining VMs.

## 4. Networking
### Virtual network (VNet)
The most fundamental part of Azure and connects all resources.

### Load Balancer
Load Balancer distributes network traffic across resources or servers. 

### VPN Gateways
VPN Gateway is a specific VNet Gateway that securely connects Azure resources
and on-premise networks.

### Application Gateway
Application Gateway is a type of load balancer with multiple additional features and works on the HTTP request of the traffic instead of the IP address and port.

### Content Delivery Network (CDN)
CDN is a distributed network of servers that speeds up the Internet by keeping content in locations closer to a user.

### ExpressRoute
ExpressRoute is a private and fast connection between Azure and on-premise networks. It does not go through the Internet.
## 5. Storage
### Intro
- Blob
- Disk 
- File
- Archive

### Blob
Storage Account - unique Azure namespace

Storage Levels: storage account -> conainers -> Blobs

Blob storage is a mix of items:
- images
- video
- log files
- data store (backup, restore, archives)

Three types of blobs:
1. Block - text and binary data up to 4.7 TB; managed individually
2. Append - optimized for append operations; logging data for VMs
3. Page blobs - up to 8TB

Pricing tiers:
- Hot 
- Cool
- Archive

### Disk
Disk that is managed by VM

Types:
- HDD for backups
- SSD standard for production
- Premium SSD better than standard
- Ultra Disk for most demanding apps,
extremely scalable, up to 64TB

### File
File storage account benefits
- easy sharing
- managed hardware and OS
- resilient to network issues

Useful scenarios for using file storage:
- hybric - supplement or replace existing on-premise 
file storage
- lift and shift - move existing file storages and related services to Azure

### Archive
Overview:
- lowest price
- durable, encrypted, stable
- perfect for infrequent access
- free up premium storage
- secure so any personal data can be stored
- it is a blob storage, so tools that apply to Blobs
are used with Archive storage

## 6. Database

## 7. Authentication and Authorization

## 8. Azure Solutions

## 9. Security

## 10. Privacy, Compliance and Trust

## 11. Pricing

## 12. Support