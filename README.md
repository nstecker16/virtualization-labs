# Virtualization Labs
Creating a Windows Server lab environment using Proxmox VE.

## Setup
I installed Proxmox VE 9 on my old gaming desktop using the [official Proxmox documentation][proxmox-install-docs] as a guide.  

### Desktop Hardware Specs
Motherboard: MSI Z97S SLI Krait Edition  
Processor: Intel(R) Core(TM) i5-4690K CPU @ 3.50GHz  
RAM: 8 GiB DIMM DDR3  
Storage: WDC WD10EZEX-60Z 1TB (931 GB usable)  
GPU: GeForce GTX 750 TI  

### Access
I am accessing the Proxmox VE web UI on my main desktop via Ethernet connections between the two desktops and an old router which is acting as a switch.  

## Objectives
Create a functioning Windows Server environment including a router, Windows Server machine with an Active Directory domain controller, and several Windows 11 user machines.

## Environment

### Machines

#### Naming/ID Conventions
Machines should be named according to the OS or image that is installed on the machine followed by a number noting the instance of that image  
For example:  
- windows11-1 would be the first instance of a machine running the Ubuntu OS  
- windows11-2 would be the second Ubuntu instance  

Machines should be given container IDs based on the final byte in their IP address  
- The range of addresses allotted for Proxmox VMs is xx.xx.xx.202-255  
- xx.xx.xx.201 is the address for the Proxmox node  

### Networking

#### Topology
![Network Topology](./proxmox-topology.png)  

#### IP Addressing

### Services

[paste links below here]: #

[proxmox-install-docs]: https://pve.proxmox.com/pve-docs/pve-admin-guide.html#chapter_installation  