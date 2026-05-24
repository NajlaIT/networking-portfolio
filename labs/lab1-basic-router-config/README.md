# Lab 1: Basic Router Configuration

## Overview
This lab demonstrates basic router configuration using CLI commands. It includes setting up a router interface, assigning an IP address, enabling the interface, and verifying network connectivity.

## Objective
- Understand basic router configuration
- Configure a router interface with an IP address
- Bring up the interface using `no shutdown`
- Verify connectivity using `ping`

## Tools Used
- Cisco Router (CLI)

## Configuration Steps

### 1. Enter privileged mode
Router> enable

### 2. Enter global configuration mode
Router# configure terminal

### 3. Select interface
Router(config)# interface gigabitEthernet0/0

### 4. Assign IP address
Router(config-if)# ip address 192.168.1.1 255.255.255.0

### 5. Enable interface
Router(config-if)# no shutdown

## Verification
- Interface status changed to **up/up**
- Successful ping responses confirmed connectivity between devices

## Key Learnings
- Basic router configuration using CLI
- Importance of interface activation using `no shutdown`
- Understanding IP addressing and subnet masks
- Interface status concepts (up/up, down/down)

## Result
The router interface was successfully configured, and network connectivity was verified using ping tests.

## Notes
This lab is part of a structured networking portfolio aimed at building foundational networking and routing skills.
