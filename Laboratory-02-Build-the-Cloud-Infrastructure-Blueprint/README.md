# Laboratory 02 – Build the Cloud Infrastructure Blueprint

## Mission Overview

The mission of this laboratory is to understand the basic components of cloud infrastructure and how they work together. The laboratory involved investigating a Linux cloud server using KillerCoda, identifying compute, storage, networking, and operating system resources, comparing major cloud providers, and designing a simple cloud infrastructure for a fictional company.

---

## Objectives

The objectives of this laboratory are:

1. Investigate and document the resources available in a Linux cloud environment.
2. Identify compute, storage, networking, and operating system components.
3. Understand the purpose and importance of each cloud infrastructure component.
4. Compare the infrastructure services offered by AWS, Microsoft Azure, and Google Cloud Platform.
5. Create a simple cloud infrastructure blueprint.
6. Practice documenting technical information using Markdown.

---

## Cloud Infrastructure Components

The following cloud infrastructure components were identified during the laboratory:

| Component | Example | Purpose |
|---|---|---|
| Compute | Intel Xeon E312xx CPU with 1 CPU core | Provides processing power for applications and tasks |
| Storage | `/dev/vda1` with 19G capacity | Stores the operating system, applications, and files |
| Networking | `enp1s0` with IP `172.30.1.2` | Provides network communication |
| Operating System | Ubuntu 24.04.4 LTS | Manages hardware and software resources |

### Compute Resources

The KillerCoda server uses an Intel Xeon E312xx processor with one CPU core and 1.9 GiB of RAM. These resources allow the Linux environment to execute commands and run applications.

### Storage Resources

The main storage device is `/dev/vda1`, which has a capacity of 19G and uses the ext4 file system. It provides storage for the operating system, applications, and files.

### Networking Resources

The main network interface is `enp1s0`, which uses the IP address `172.30.1.2`. Networking allows the server to communicate with other systems and services.

### Operating System

The server runs Ubuntu 24.04.4 LTS with Linux kernel version `6.8.0-136-generic`. The operating system manages the available hardware and provides an environment for running applications and commands.

---

## Tools Used

The following tools were used during the laboratory:

- **KillerCoda** – Used to access and investigate the Linux cloud environment.
- **Linux Terminal** – Used to execute system investigation commands.
- **GitHub** – Used to store and organize the laboratory files.
- **Markdown** – Used to create the technical documentation.
- **Draw.io / Diagramming Tool** – Used to design the cloud infrastructure diagram.
- **Web Browser** – Used to research AWS, Microsoft Azure, and Google Cloud Platform documentation.

---

## Linux Commands Executed

The following Linux commands were used to investigate the cloud server:

| Linux Command | Purpose |
|---|---|
| `cat /etc/os-release` | Identifies the operating system |
| `uname -r` | Displays the Linux kernel version |
| `lscpu \| grep "Model name"` | Displays the CPU model |
| `nproc` | Displays the number of CPU cores |
| `free -h` | Displays RAM information |
| `df -h` | Displays disk capacity and usage |
| `findmnt` | Displays mounted file systems |
| `hostname` | Displays the server hostname |
| `hostname -I` | Displays the IP address |
| `ip addr` | Displays network interfaces and IP addresses |

### Important Results

| Information | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Kernel | 6.8.0-136-generic |
| CPU | Intel Xeon E312xx |
| CPU Cores | 1 |
| RAM | 1.9 GiB |
| Main Disk | 19G |
| Hostname | ubuntu |
| IP Address | 172.30.1.2 |

---

## Skills Learned

During this laboratory, I learned how to:

- Investigate a Linux cloud server using terminal commands.
- Identify CPU, RAM, storage, and networking resources.
- Check the operating system and Linux kernel version.
- Identify mounted file systems.
- Determine the hostname and IP address of a Linux server.
- Understand the relationship between compute, storage, networking, and operating systems.
- Compare equivalent infrastructure services from AWS, Microsoft Azure, and Google Cloud Platform.
- Create a simple cloud infrastructure diagram.
- Organize and document a technical project using GitHub and Markdown.

---

## Challenges Encountered

One challenge encountered during the laboratory was understanding the different Linux commands used to investigate the server. Some commands produced detailed information that required careful reading to identify the important values.

Another challenge was understanding that AWS, Microsoft Azure, and Google Cloud Platform provide similar infrastructure services but use different names for those services. Creating the cloud infrastructure diagram also required deciding how the user, internet connection, network, compute resource, and storage resource should be connected.

Despite these challenges, the laboratory helped improve my understanding of cloud infrastructure and Linux server administration.

---

## Laboratory Files

The laboratory contains the following files:

- [`infrastructure-report.md`](infrastructure-report.md) – Linux server investigation
- [`cloud-components.md`](cloud-components.md) – Cloud infrastructure components
- [`cloud-provider-comparison.md`](cloud-provider-comparison.md) – AWS, Azure, and GCP comparison
- [`reflection.md`](reflection.md) – Laboratory reflection

### Screenshots

The investigation screenshots are stored in the `screenshots` folder:

- `server-information.png`
- `network-information.png`
- `storage-information.png`
- `cloud-architecture.png`
