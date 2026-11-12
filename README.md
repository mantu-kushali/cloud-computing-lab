# Cloud Computing Lab

This repository contains my weekly lab submissions for the Cloud Computing Lab course.

**Name:** Mantu Kushali
**Repository:** Weekly lab reports (PDF) for each assignment, organized by week.

## Structure

```
cloud-computing-lab/
├── Week1/
│   └── Lab1_Report.pdf
├── Week2/
│   └── Lab2_Report.pdf
├── Week3/
│   └── Lab3_Report.pdf
│
└── README.md
```

## Lab 1 — VirtualBox VM Setup

- Installed Oracle VirtualBox (hypervisor)
- Created a new VM (Ubuntu_VM) with 4096 MB RAM, 2 CPUs, and a 25 GB disk
- Attached the Ubuntu 25.04 ISO image and completed the guest OS installation
- Verified the VM boots successfully into the Ubuntu desktop
- Installed `build-essential` and matching Linux kernel headers inside the guest OS

Full details and screenshots are in `Week1/Lab1_Report.pdf`.

## Lab 2 — TCP Client-Server Chat

- Set up two Ubuntu VMs connected through a VirtualBox internal network
- Server VM IP: `192.168.10.1`, Client VM IP: `192.168.10.2`
- Ran a TCP client-server chat program between the two VMs

Full details and screenshots are in `Week2/Lab2_Report.pdf`.

## Lab 3 — Simple Network Topology using Mininet

- Used Mininet 2.3.0 on an Ubuntu VM running in VirtualBox
- Created the default topology: 1 Open vSwitch bridge (`s1`) and 2 hosts (`h1` = 10.0.0.1, `h2` = 10.0.0.2)
- Inspected the network with `nodes`, `net`, `dump` and `links`
- Tested connectivity with `pingall` (0% dropped) and `h1 ping -c 4 h2` (4/4 packets received)
- Stopped the network with `exit` and cleaned up with `sudo mn -c`

Full details and screenshots are in `Week3/Lab3_Report.pdf`.