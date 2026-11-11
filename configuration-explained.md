
# Cisco Switch Configuration Explained

This document explains the main settings used in my Cisco Catalyst switch configuration example.

## VLAN Configuration

VLANs help separate devices into different networks.

In this example:
- VLAN 10 - Users
- VLAN 20 - Servers
- VLAN 30 - Printers
- VLAN 99 - Management

## Access Ports

Access ports are used to connect devices such as computers and printers.

Each access port belongs to a specific VLAN.

## Trunk Ports

Trunk ports carry traffic from multiple VLANs between switches or other network devices.

## Port Security

Port security helps control the number of devices allowed on a switch port.

It can also restrict traffic when a security violation occurs.

## Spanning Tree

Rapid PVST helps prevent network loops and supports faster recovery when network connections change.

## Switch Management

A management IP address is used to access the switch remotely.

SSH provides secure remote access when authentication is properly configured.

## Network Monitoring

SNMP can be used with tools such as SolarWinds to monitor switch availability and interface status.

## Troubleshooting Commands

| Command | Purpose |
|---|---|
| `show vlan brief` | Check VLANs |
| `show interfaces status` | Check connected ports |
| `show interfaces trunk` | Check trunk ports |
| `show spanning-tree` | Check spanning-tree status |
| `show ip interface brief` | Check interface IP addresses |
| `show logging` | Check switch logs |

## Note

The configuration in this repository is a simplified example. It does not contain real company network details.
