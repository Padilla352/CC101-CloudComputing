# Cloud Storage Types Research

## Block, File, and Object Storage

Cloud environments commonly use three major types of data storage: block storage, file storage, and object storage. Each type is designed for different workloads and access patterns.

| Storage Type | Description | Common Use Cases | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be accessed independently. | Virtual machine disks, databases, and applications requiring low-latency storage. | Amazon EBS |
| File Storage | Stores data as files organized in directories and folders using a hierarchical structure. | Shared files, content management, home directories, and applications requiring a shared file system. | Amazon EFS |
| Object Storage | Stores data as objects together with metadata and a unique identifier. | Images, videos, backups, archives, documents, and other unstructured data. | Amazon S3 |

## Block Storage

Block storage divides data into blocks and provides applications with storage that behaves similarly to a disk. It is commonly used for virtual machine operating systems, databases, and workloads that require low-latency access.

## File Storage

File storage organizes data into files and directories. It is useful when multiple systems or users need to access shared files through a familiar file-system structure.

## Object Storage

Object storage stores each piece of data as an object along with metadata and a unique identifier. It is well suited for large amounts of unstructured data such as photos, videos, backups, and archives.

## Client Explanation

For a client storing large numbers of photos, object storage would be an appropriate choice because photos are unstructured files that can be stored as individual objects. Object storage is also designed to scale to large amounts of data and can store metadata with each object.

## Sources

- Amazon Web Services. "What’s the Difference Between Block, Object, and File Storage?"
- Amazon Web Services. "Choosing an AWS Storage Service."
- Amazon Web Services. "Amazon S3."
- Amazon Web Services. "Amazon EBS."
- Amazon Web Services. "Amazon EFS."
