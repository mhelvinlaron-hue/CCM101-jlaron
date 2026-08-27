# CCM101 Multi-Cloud Explorer

## Project Overview
This project is part of the CCM101 Cloud Computing laboratory activity. It focuses on exploring AWS, Microsoft Azure, and Google Cloud Platform and comparing how their services can be used for different cloud computing needs.

## Cloud Platforms

### Amazon Web Services
AWS is a major cloud platform that provides services for computing, storage, networking, databases, security, and application development. It is known for its large number of available cloud services and worldwide infrastructure.

### Microsoft Azure
Microsoft Azure is Microsoft's cloud computing platform. It is commonly used by organizations that already work with Windows Server, Microsoft 365, and other Microsoft technologies.

### Google Cloud Platform
Google Cloud Platform provides cloud services for computing, storage, networking, data processing, artificial intelligence, machine learning, and Kubernetes based applications.

## Linux Server Investigation
The Linux environment was examined using commands such as `lsb_release -a`, `lscpu`, `free -h`, and `df -h`.

### Operating System
The server is running **Ubuntu 24.04.4 LTS**, with release version **24.04** and codename **noble**.

### CPU
The server uses an **Intel Xeon E312xx processor** based on the Sandy Bridge architecture. It has **1 CPU core**, uses the **x86_64 architecture**, and runs under the **KVM hypervisor**.

### Memory
The system has **1.9 GiB of RAM** in total. At the time of the investigation, **428 MiB was being used**, with approximately **1.4 GiB available**. It also has **1.0 GiB of swap space**.

### Disk Space
The main filesystem, `/dev/vda1`, has **19 GB of storage**. Around **5.4 GB is currently used**, while approximately **13 GB remains available**. The main partition is **30% full**.

There are also separate partitions for `/boot` and `/boot/efi`.

## Cloud Migration Analysis
If this Linux server were moved to the cloud, it could be hosted using **Amazon EC2, Azure Virtual Machines, or Google Compute Engine**. The server has relatively low resource requirements, so a small virtual machine would be enough for basic applications, testing, and learning. Among the three platforms, I would choose **Amazon EC2** because it provides different instance sizes and would give me practical experience with AWS.

## Cloud Service Comparison

| Service Category | AWS | Azure | GCP |
|---|---|---|---|
| Virtual Machine | EC2 | Azure Virtual Machines | Compute Engine |
| Object Storage | S3 | Blob Storage | Cloud Storage |
| Identity Management | IAM | Microsoft Entra ID | Cloud IAM |
| SQL Database | Amazon RDS | Azure SQL Database | Cloud SQL |
| Kubernetes | Amazon EKS | Azure Kubernetes Service | Google Kubernetes Engine |

## Client Recommendations

### Client A: Startup Company
**Recommended Platform:** Google Cloud Platform
A startup can use GCP to begin with smaller resources and increase them as its customer base grows. This can help the company avoid purchasing expensive physical hardware at the beginning.
**Services:** Compute Engine, Cloud Storage, Cloud SQL

### Client B: University
**Recommended Platform:** Microsoft Azure
Azure is suitable for the university because it already uses Microsoft technologies. Azure can work with existing Windows systems and Microsoft identity services.
**Services:** Azure Virtual Machines, Microsoft Entra ID, Azure Storage

### Client C: AI Research Company
**Recommended Platform:** Google Cloud Platform
GCP is a good fit for an organization working with artificial intelligence and machine learning. Its computing and AI services can support model development, training, and deployment.
**Services:** Vertex AI, Compute Engine, Cloud Storage

### Client D: Global E-Commerce Company
**Recommended Platform:** Amazon Web Services
AWS is suitable for an international online store because it provides services for scaling applications, distributing traffic, and delivering content to users in different locations.
**Services:** Amazon EC2 Auto Scaling, Elastic Load Balancing, Amazon CloudFront
