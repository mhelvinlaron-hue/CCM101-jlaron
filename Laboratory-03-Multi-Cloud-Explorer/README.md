# Laboratory Activity 3: Multi-Cloud Explorer

## Linux Investigation

### Operating System
Ubuntu 24.04.4 LTS

### CPU Information
Intel Xeon E312xx (Sandy Bridge, IBRS update), 1 CPU core, x86_64 architecture. The system is running under the KVM hypervisor.

### Memory
1.9 GiB total RAM, with 428 MiB used and approximately 1.4 GiB available. The system also has 1.0 GiB of swap space.

### Disk Space
19 GB total on `/dev/vda1`, with 5.4 GB used and approximately 13 GB available. The main filesystem is 30% used.

## Cloud Migration Analysis

**If this Linux server were migrated to the cloud, which AWS, Azure, and GCP services could host it?**

If this Linux server were migrated to the cloud, it could be hosted using Amazon EC2, Azure Virtual Machines, or Google Compute Engine. Since the server only has one CPU core and about 2 GB of RAM, a small virtual machine would be enough for its workload. I would choose Amazon EC2 because it provides flexible instance options and would be useful for practicing cloud server management.
