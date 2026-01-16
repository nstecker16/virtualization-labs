# OPNSense Configuration

## Guide

Utilized [this guide][opn-sense-configuration]

## Configuration

- Login
    - user: root
    - pass: opnsense-1

### Virtual Hardware

- 4 GB RAM
- 1 CPU socket, 4 cores
- 20 GB disk storage

### Network Interfaces

- vtnet0
    - Utilizing Proxmox bridge [vmbr0](/proxmox-env/bridges.md#vmbr0)
- vtnet1
    - Utilizing Proxmox bridge [vmbr1](/proxmox-env/bridges.md#vmbr1)

[paste links below here]: #

[opn-sense-configuration]: https://thetechguy.it/post/35-home-lab-opnsense-installation/