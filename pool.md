# Notes for AZ-900: Microsoft Azure Fundamentals exam
# Cloud Academy
## 1. Introduction to the cloud
### What is Cloud Computing?
The cloud is rapidly developing technology. 
It helps companies to operate on a huge scale.  

Cloud Computing is a remote virtual pool of on-demand
shared resources offering Compute, Storage, Database, and
Network services that can be rapidly deployed at scale.

The word **SCALE** is crucial here. 

Cloud is based on a on-premise technology. So it solves
problems that are related to on-premise. It maximizes the power of cloud computing.

What is **Virtualization**?
You can have multiple virtual machines, each running a separate OS and applications using 1 physical server!
This is huge.

**Sharing hardware resources** is a key here.

A **hypervisor**, which is a piece of software, allows to create multiple VMs to be installed on the same physical server.

Any request to the hardware goes via the Hypervisor. 

Benefits of Virtualization:
- less hardware is required (reduced capital expenditure)
- less space, power, cooling required within datacenter (reduced operating costs)
so **optimization of resources** 

**Virtualization** has been used in on-premise datacenters for a long time.

What are resources?
- Compute 
- Storage 
- Database
- Network

* Compute
Compute objects are like 'brains' to process workloads.
CPUs, RAM, related to hardware

* Storage
resource that allows me to save and store the data
- typical env -> hard disk

* Database
What are databases?
not much info
engines SQL, MySQL

* Network resource
connectivity between resources having some function
e.g. routers to route traffic, fire walls to allow or deny traffic

'Cloud Computing' is a remote virtual pool of on-demand
shared resources offering Compute, Storage, Database, and Network services that can be rapidly deployed at scale.

### Cloud Deployment Models

- Public Cloud
- Private Cloud
- Hybrid Cloud

**Public Cloud**
A vendor gives access to the infrastructure
It can be provisioned on demand
exact location is not known to a consumer but the region is known.

The cloud vendor gives all the bacend and physical maintenance such as power, cooling, hardware failures.

You can access a public cloud from anywhere you just need an internet connection.

**Private Cloud**
Infrastructure is privately hosted and managed.
More direct control, security.
The hardware is on-premise.

But is different from the typical *on-premise server farm*
Still Virtualization, sharing compute, storage, network
Virtualization will create a pool of shared compute. storage and network resouces.

More capital expenditure is required
opex also increases
Capital expenditure?
CapEX; investments on start
OpEX; running costs

**Hybrid Cloud**
Public and Private Cloud
for seasonal high-load traffic or Disaster Recovery
it is a link between private and public cloud

hybrid is often short-term config for test and dev

public/private/hybrid vs. security/data location/capital expediture/operational expedinture/tenancy

Key Cloud Concepts
- On-demand resourcing - immediate provisioning

- Scalability - scaling up; scaling down; 'in and out'
use more computing power or less; num

up/down - more computing resources per virtual machine
in/out - add or remove the number of VMs

great advantage in comparison to in-promise

- economy of scale 
low resource costs compared to traditional hosting

- flexibility and elacticity
you choose the amount of resources you requires, how much; how long; what scale
custimization

- growth 
organization with the benefits off cloud can grow easily

- utility based metering
pay for what you use

- shared infrastructure
multiple organizations/users - tenants can be running VMs on the same hardware

less physical hardware; cheaper you know

- highly available
?? do not understand the slide

- security
AWS and Azure considered to be more secure
shared responsibility model

### Cloud Service Models
IaaS; PaaS; SaaS
different level of managibility and customization

- Software as a Service (SaaS)
the least customizable
widley distributed and  accessed Gmail

- Platform as a Service (PaaS) 
greater level of control

access to a framework; but underlying architecutre; physical hardware, network component, and OS are typically managed by the vendor

- Infrastructure as a service (IaaS)
the greates level of customization and control

you configure your own resources, VMs, virtual networks; OS etc.

vendor controls hardware
other:
DRaaS, CaaS, etc.

### Common use cases of Cloud Computing
- Migration from on-premise to public cloud

- Traffic Bursting
using to cloud to manage traffic in hard seasons

- Backup/Disaster Recovery
unlimited storage space

- Web Hosting
load balancers are good, traffic deloading; scaling
CDN is amazing; cashing locally

- Test/Dev Env
use servers for test and dev when u need

- Proof of Concept
prepared sucessful solutions? 

- Big Data/Data Manipulation
huge datasets; data lakes; good way to manage them

### Mapping data center architecture to the cloud alternative
i'd like to run my own small data center and pet it like a puppy;
- location; 1 office; cloud many places
- physical security 
public cloud vendor's responsibility is to make it secure; you need less
- mechanical and electrical infrastructure
cooling; air conditionin; fire supression; etc.
- network infrastructure
switching, routers; firewalls
cloud has easily to set up networks
- servers 
they are virtual machines
- storage
unlimited, scalable; great
storage area network

### Summary
Cloud computing
remote virtual pool of on-demand shared resources offering Compute, Storage, Database, and Network services that can be rapidly deployed at scale.

* based on virtualized tech
* resources Compute, Storage, Database, Network
CSDN
CNDS

3 cloud deployment models
public/private/hybrid

key terms
on-demand/scalability/economy-of-scale/flexibility&elasticity/growth/pay-as-you-go/shared-infrastructure/highly-available/shared-security

3 service models
IaaS/PaaS/SaaS

uses of cloud comp
migration/traffic bursting/backup-dr/test-dev/proof-concept/data


* read about shared responsibility model
**VIRTUAL RESOURCE SCALE**

## Overview of Azure Services
Microsoft Azure is a collection of services that organizations can use.

Azure has its own datacenters, don't need to have it, maintain infra and scale resources for you.

## Compute
- Azure VMs  
'lift and shift' migration
from on-premise to virtual
IaaS

- Azure App Service - PaaS  
but... if it's not a mobile or web app then cannot use AAS

- Azure Container Instance  
self-contain software env e.g., complete app + all dependencies  
containers are like VMs but they don't include OS
use Azure Container Instance to run container using a single command

but when more complex applications then
- Azure Kubernetes Service  
easy to deploy and manage multi-container apps

- Azure Functions  
something like Azure Apps but you use to do single task and you pay only when it gets used

## Storage
- Azure Blob Storage  
object storage; collection of files; no hierarchical folder structure; it's flat, for videos, images, etc.
HOT (frequent), COOL (infrequent), ARCHIVE (backup, lowest cost)  
if you need hierarchical file storage

- Azure File Storage  
hierarchical structure; files for Windows servers

- Azure Data Lake Storage Gen2  
Hadoop-compatibile for data analytics apps

- Azure SQL databases  
relational databases, very similar to sql server; open source version are also available:

- Azure DB Open Source   
Azure Database for MySQL, Azure Database for Maria DB, Azure Database for PostgreSQL online transactions processing; on

I really like the transistions between learned concepts

- Azure Synapse Analytics  
data warehouse; integration of many services

- Azure Cosmos DB
SQL Database not enough; the traffic to high so use Azure Cosmos DB; NoSQL, not relational; sacraficing some power to meet demand of users

Cosmos DB can scale globally

- Azure Cache for Redis  
can speed application's data by 
caching frequently requested data
cashing caching - almost funny
caching is important; is like storing data/files closer to the users

## Networking
- Azure Virtual Network (VNet)  
similar to on-premise;
each VM in VNet gets IP address and can be communicated with other VMs
Communication between VMs; VMs - the 

- Subnets  
You can divide VNets into subnets and route them;
in-bound traffic

- VNet peering
communications between VNets; or to be more exact; communication between VMs in one VNet and VMs in another VNet; other resources such as Kubernetes clusters can be in VNets too; VM is just a simple example of a resource

- Azure VPN
Secure connection between VNet and on-premise networks a) Virtual Private Network is on-premise -- encrypted traffing in the public Web -- VNet b) ExpressRoute on-premise --dedicated, fast and reliable connection -- VNet; but of course ExpressRoute is expensive 

## Using the Azure Portal
There are many ways to interact with Azure
- Azure Portal (Web, mobile app)
- Azure CLI
- Azure PowerShell
- SDK (Java, JavaScript, Python, etc.)

SDK is needed if you do some programming in some programming langugae and want to interact with Azure


### Use Azure Portal to create a resource -> VM
Microsoft creates Billing Account and Subscription, both involved in billing

BASICS
- **Billing Account**    
is an your agreement or orgniazation's agreement to use 
- **Subscription**  
a collection of all of resources you use 

you may want multiple subscriptions in one billing account; 
each subscription generates a seperate invoice; it is good to have separate subscriptions for security or other reasons

- **Resource Group**  
a collection of resources, like subscription; but subscription can have multiple resource group.

- **Location**  
regions, availability zones;
region that supports availability zones has at least three data centers. It is good to put VMs in different zones. If one is loaded, has troubles other still work.

- Image
Ubuntu Server example

- Size

- Administrator account
best to use ssh

- inbound port rules
access from the internet

DISKS  
hdd/ssd/premium etc

NETWORK
default -> vnet, subnet, and public IP address

**mini-tutorial on web app??**

## Service Categories
Other important services than those related to compute, storage, networking, database

### Migration
Azure Migrate helps organizations migrate to the cloud.  
What does Azure Migrate do?
I Discovers on-premise; physical, virtual
II Assesses the machines;
III It assesses if it's good a condition to migrate; shows costs
integrated with other tools
It is easy to integrate Active Directory with Azure Active Directory,
so migration of identities is possible.

### DevOps
the idea is that you can **automate** many stages of application building:
dev stage/testing/production.

The most important
- **Azure Pipelines** allows to create automated workflows to build, test, and deploy

- Azure DevTest Labs helps to organize non-production env; so developing is testing is autometed, quicker, better;

- Azure Content Delivery Network (it is in DevOps category?? why?)
caches frequently accessed content and brings it to serveres closer to a web user

### Internet of Things (IoT)
many devices connected to the cloud

- Azure IoT Central (SaaS)  
creating IoT app without any code

- Azure IoT Hub  
you have more control; IoT Central uses it 

- Azure Sphere   
gives layers of protection

---Day 3---

### Analytics
- Azure HDInsight  
Supports open-source bigdata frameowkrs such as Hadoop. Spark, etc.

- Azure Databricks  
a more user-friendly

- Azure Synapse Analytics  
more integration, combines data warehouse func with
Apache Spark support

### AI (machine learning)  
learning; training the model to make a prediction

- Azure Cognitive Services  
a collection of ready-to-use AI tools; you can add it
to applications without extensive knowledge of AI;
five categories: decision, language, speech, vision, web search;

- Azure Bot Service

- Azure Machine Learning Studio  
build, train ML models without coding  

- Azure Machine Learning Services  
fine-grained control; etc. train models 
using Azure Databricks, deploy with Azure Kubernetes Service; the best solution if you want to build your own custom AI app;

### Integration

- Azure Logic Apps and Azure Event Grid  
can create complex workflows using many 3-party apps;


# A Cloud Guru
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

### Identity types
Not everyone can get access to some of the resources

Authentication is a confirmation of your identity:
user
password

first test

Authorization
after authentication
granual access

### Azure Active Directory
Main tool to managa users and permissions

Tenant - dedicated instance of AAD for specific organization

each tenant is distinct and completely separate from AAD

each user max in 500 tenents
every user is a member of at least 1 tenant

# Multi-Factor Authentication
More form of authentications
- Something you know
- Something you have
- Something you are

# Azure Active Directory Seamless Single Sign-On ???
Use single user and password for every app


## 8. Azure Solutions
Examples of other Azure Services
### Internet of Things
Complex network of connected things and people.
Things and people send data about them.

Example: IoT in transport; Google knows where is the traffic

**Azure IoT Hub**
PaaS

**IoT Central** 
SaaS

**Azure Sphere**

### 

## 9. Security

## 10. Privacy, Compliance and Trust

## 11. Pricing

## 12. Support