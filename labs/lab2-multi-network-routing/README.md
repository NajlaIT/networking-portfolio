# Lab 2: Multi-Network Design and Inter-Network Routing

## Overview
This lab demonstrates how a router enables communication between two different networks. The network was designed using multiple PCs, switches, and a router to simulate a small multi-network environment.

## Objective
- Configure multiple networks using different IP ranges
- Assign IP addresses and default gateways to end devices
- Configure router interfaces
- Enable communication between separate networks
- Verify routing functionality using ping tests

## Network Design

### Network A
- Network: 192.168.10.0/24
- Gateway: 192.168.10.1

### Network B
- Network: 192.168.20.0/24
- Gateway: 192.168.20.1

## Devices Used
- 1 Router
- 2 Switches
- 4 PCs

## Router Configuration

### Interface G0/0
Router(config)# interface gigabitEthernet0/0
Router(config-if)# ip address 192.168.10.1 255.255.255.0
Router(config-if)# no shutdown

### Interface G0/1
Router(config)# interface gigabitEthernet0/1
Router(config-if)# ip address 192.168.20.1 255.255.255.0
Router(config-if)# no shutdown

## Verification
- Router interfaces successfully reached up/up state
- Devices in different networks successfully communicated using ping
- Cross-network connectivity was verified

## Key Learnings
- Basic inter-network routing concepts
- Importance of default gateways
- Network segmentation using different subnets
- Router interface configuration and verification
- End-to-end connectivity testing

## Result
The router successfully routed traffic between two separate networks, allowing devices from different subnets to communicate with each other.

## Notes
This lab is part of a structured networking portfolio focused on building practical networking and routing skills.
