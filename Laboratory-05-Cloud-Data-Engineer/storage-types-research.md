# Research: Types of Cloud Storage

Research: Types of Cloud Storage

Storage TypeDescriptionPrimary Use CaseCloud Provider Example

Block Storage

Divides data into fixed-size blocks, with each block having its own address. It works like a virtual hard drive that can be connected to a server.

Commonly used for operating systems, databases, and applications that require fast and reliable disk performance.

AWS EBS (also Azure Managed Disks, Google Persistent Disk)

File Storage

Organizes data into files and folders within a directory structure. It can be shared across a network using protocols such as NFS or SMB.

Useful for shared folders, content management systems, home directories, and applications that need access to the same files.

AWS EFS (also Azure Files, Google Filestore)

Object Storage

Stores data as individual objects, with each object containing the data, metadata, and a unique identifier. It is commonly accessed through HTTP and APIs.

Best suited for large amounts of unstructured data, including photos, videos, backups, documents, and system logs.

AWS S3 (also Azure Blob Storage, Google Cloud Storage)

Why Object Storage for the Client's Photos

Object Storage is a suitable choice for the client's photo-sharing application because it can handle a very large number of images without requiring the application to manage physical disks or storage capacity. Each photo is stored separately as an object and can include its own metadata. Photos can also be uploaded and accessed through HTTP using an S3-compatible API.



Compared with block storage, which is connected to a specific server, and file storage, which uses shared folders and directories, object storage is more scalable and flexible for handling millions of photos. It is also designed for durability and can operate independently from the web server or application container.

