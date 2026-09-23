# Cloud Storage Types Research

Cloud storage can be divided into three common types: Block Storage, File Storage, and Object Storage. Each type is designed for different purposes and workloads.

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be attached to a virtual machine and used like a traditional hard drive. | Operating systems, databases, and applications that require fast and direct storage access. | AWS EBS |
| File Storage | Stores data as files organized in folders and directories. Multiple systems or users can access the same file storage. | Shared files, documents, team folders, and applications that need a shared file system. | AWS EFS |
| Object Storage | Stores data as objects together with metadata and a unique identifier inside containers called buckets. | Images, videos, backups, logs, and other large amounts of unstructured data. | Amazon S3 |

## Why Object Storage is the best choice for storing their user-uploaded images.

Object Storage is a good choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images and videos. It can also scale as the number of uploaded photos increases, making it suitable for an application that may need to store millions of user-uploaded images.
