# Cloud Storage Types Research

Cloud storage can be divided into three common types: Block Storage, File Storage, and Object Storage. Each type is designed for different workloads and storage requirements.

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                                                                                                                 | Primary Use Case                                                                                | Cloud Provider Example                 |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | -------------------------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be accessed individually. It behaves similar to a traditional hard drive or disk attached to a server.            | Operating systems, databases, and applications that require fast and consistent disk access.    | Amazon Elastic Block Store (AWS EBS)   |
| **File Storage**   | Stores data in files and folders using a shared file system. Multiple systems can access the same files through the network.                                | Shared documents, application files, and workloads that require a traditional folder structure. | Amazon Elastic File System (AWS EFS)   |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. Objects can include images, videos, documents, backups, and other unstructured data. | Large amounts of unstructured data such as photos, videos, backups, and static website files.   | Amazon Simple Storage Service (AWS S3) |

## Why Object Storage is Suitable for the Client

Object Storage is a good choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images. It also allows files to be accessed through APIs and can scale as the number of uploaded photos increases.
