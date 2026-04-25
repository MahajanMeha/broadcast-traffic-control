# Broadcast Traffic Control using Mininet & Open vSwitch

## Name: Meha Mahajan

## SRN: PES2UG24AM090

### Objective

To detect and control broadcast traffic using OpenFlow rules.

### Tools Used

* Mininet
* Open vSwitch
* Ubuntu
* tcpdump

### Description

This project demonstrates how broadcast traffic is generated, detected, and controlled using SDN concepts.

### Key Commands

* `sudo mn --topo tree,depth=2,fanout=2 --controller=none`
* `h1 ping -b 10.0.0.255`
* `sudo tcpdump -i any`
* `sudo ovs-ofctl add-flow s1 "priority=100,dl_dst=ff:ff:ff:ff:ff:ff,actions=drop"`

### Result

Broadcast traffic is reduced by applying flow rules.

---
