# Project Overview
A Cisco Packet Tracer basic LAN configuration project based on the supplied topology. The network uses the 172.16.0.0/16 address space and includes one router, two switches, and four PCs.
Topology
R1 connects to SW1. SW1 connects to PC1, PC2, and SW2. SW2 connects to PC3 and PC4.

## Device	Interface	IP Address	Subnet Mask	Default Gateway
R1	G0/0	172.16.0.254	255.255.0.0	—
PC1	Fa0	172.16.0.1	255.255.0.0	172.16.0.254
PC2	Fa0	172.16.0.2	255.255.0.0	172.16.0.254
PC3	Fa0	172.16.0.3	255.255.0.0	172.16.0.254
PC4	Fa0	172.16.0.4	255.255.0.0	172.16.0.254
