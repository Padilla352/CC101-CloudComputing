# Cloud Infrastructure Components

## 1. Compute Resources

### Example Found in the KillerCoda Linux Environment

The compute resource found in the KillerCoda Linux environment is the CPU.

- CPU Model: Intel Xeon E312xx (Sandy Bridge, IBRS update)
- Number of CPU Cores: 1
- Total RAM: 1.9 GiB

### Purpose

Compute resources provide the processing power needed to run the operating system, commands, applications, and services. The CPU processes the instructions given to the computer.

### Importance in Cloud Computing

Compute resources are important in cloud computing because applications and services need processing power to operate. Cloud computing allows users to access computing resources without having to maintain their own physical servers.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux environment provides an Intel Xeon E312xx CPU with one CPU core and 1.9 GiB of RAM. These resources are used to run the Ubuntu Linux environment and the commands executed during the laboratory. The CPU information was identified using the `lscpu` command, while the number of CPU cores was identified using `nproc`.

---

## 2. Storage Resources

### Example Found in the KillerCoda Linux Environment

The storage resources found in the KillerCoda Linux environment include the main disk and mounted file systems.

- Main Disk: `/dev/vda1`
- Disk Capacity: 19G
- Main File System: ext4
- Main Mount Point: `/`
- Boot File System: `/dev/vda16`
- EFI File System: `/dev/vda15`

### Purpose

Storage resources are used to store the operating system, applications, files, and other data.

### Importance in Cloud Computing

Storage is important in cloud computing because applications and services need a place to save and retrieve information. Cloud platforms provide storage resources that can be used to store operating system files, application data, databases, and other information.

### Relation to the KillerCoda Linux Environment

The KillerCoda environment has a 19G main disk represented by `/dev/vda1`. It uses the ext4 file system and is mounted at `/`. The environment also has `/boot` and `/boot/efi` mounted file systems. These storage resources provide the space needed for the Linux operating system and its files.

The `df -h` and `findmnt` commands were used to investigate the storage resources and mounted file systems.

---

## 3. Networking Resources

### Example Found in the KillerCoda Linux Environment

The networking resources found in the KillerCoda Linux environment include the network interface and IP addresses.

- Hostname: `ubuntu`
- Main Network Interface: `enp1s0`
- Main IP Address: `172.30.1.2`
- Docker Network Interface: `docker0`
- Docker IP Address: `172.17.0.1`

### Purpose

Networking resources allow computers, servers, applications, and other systems to communicate with each other.

### Importance in Cloud Computing

Networking is important in cloud computing because cloud resources need to communicate with users, applications, databases, and other services. Networks allow data and requests to move between different cloud resources.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux environment uses the `enp1s0` network interface with the IP address `172.30.1.2`. It also has a `docker0` interface with the IP address `172.17.0.1`. These network interfaces provide connectivity within the Linux environment.

The `hostname -I` and `ip addr` commands were used to identify the IP addresses and network interfaces.

---

## 4. Operating System

### Example Found in the KillerCoda Linux Environment

The operating system found in the KillerCoda Linux environment is:

- Operating System: Ubuntu 24.04.4 LTS
- Kernel Version: 6.8.0-136-generic
- Hostname: `ubuntu`

### Purpose

The operating system manages the computer's hardware and software resources. It provides the environment needed to run applications, commands, and services.

### Importance in Cloud Computing

An operating system is important in cloud computing because cloud servers need an operating system to manage their resources and provide an environment where applications and services can run.

### Relation to the KillerCoda Linux Environment

The KillerCoda environment uses Ubuntu 24.04.4 LTS. It provides a Linux terminal where commands can be executed to investigate and manage the server's CPU, memory, storage, and network resources.

The operating system was identified using the `cat /etc/os-release` command, while the kernel version was identified using `uname -r`.

---

## Conclusion

The Linux environment provided by KillerCoda contains the basic infrastructure components needed to operate a server: compute resources, storage resources, networking resources, and an operating system.

The compute resources provide processing power, the storage resources provide space for files and system data, the networking resources provide communication, and the operating system manages the available hardware and software resources. These components work together to provide the foundation for running applications and services in a cloud environment.
