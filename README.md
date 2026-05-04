# Cisco Packet Tracer Enterprise Network Project

This academic project was developed for the Network Technologies course.  
The goal was to design, configure, document, and test a small enterprise-style network using Cisco Packet Tracer.

## Project Overview

The network simulates a small enterprise environment with multiple LAN segments connected through routers and switches.

The topology includes:

- 4 separate IPv4 LANs
- 2 Cisco 2911 routers
- 4 Cisco 2960 switches
- 12 end-user PCs
- 1 server
- Point-to-point WAN link between routers
- Static routing between networks
- DNS and HTTP services
- End-to-end connectivity testing

## Network Design

Each LAN is connected to a switch, and each switch is connected to a router interface acting as the default gateway.  
Router0 and Router1 are connected through a point-to-point WAN link.

The network was designed to demonstrate:

- IPv4 addressing
- Subnet planning
- Router and switch connectivity
- Static route configuration
- DNS name resolution
- HTTP web access
- Basic network troubleshooting

## IP Addressing Plan

| Network | Network Address | Subnet Mask | Gateway | Devices |
|---|---:|---:|---:|---|
| Network I | 192.168.1.0 | 255.255.255.0 | 192.168.1.254 | PC0, PC1, PC2 |
| Network II | 192.168.2.0 | 255.255.255.0 | 192.168.2.254 | PC3, PC4, PC5 |
| Network III | 192.168.3.0 | 255.255.255.0 | 192.168.3.254 | PC6, PC7, PC8 |
| Network IV | 192.168.75.0 | 255.255.255.0 | 192.168.75.254 | PC9, PC10, PC11, Server |
| WAN Link | 222.2.2.0 | 255.255.255.252 | - | Router0, Router1 |

## DNS and HTTP Server

A simulated DNS A record was configured inside Cisco Packet Tracer:

```text
ronikevibeden.com -> 192.168.75.10
