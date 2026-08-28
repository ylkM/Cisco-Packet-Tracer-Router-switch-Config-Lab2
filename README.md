# Cisco Basic LAN – Router & Switch Configuration

## Project Overview

This project is a basic Cisco LAN configuration completed in Cisco Packet Tracer.

The topology includes:

- 1 Cisco Router (R1)
- 2 Cisco Switches (SW1 and SW2)
- 4 PCs (PC1–PC4)
- Network: 172.16.0.0/16

The project focuses on basic Cisco IOS configuration, IP addressing, interface configuration, and network connectivity.

---

## Network Topology

`
                         172.16.0.0/16
                              |
                         R1 G0/0
                     172.16.0.254/16
                              |
                         SW1 G0/1
                              |
                +-------------+-------------+
                |                           |
            SW1 Fa0/1                   SW1 Fa0/2
                |                           |
              PC1                         PC2
        172.16.0.1/16              172.16.0.2/16


                         SW1 G0/2
                              |
                         SW2 G0/1
                         /         \
                        /           \
                   Fa0/1           Fa0/2
                     |               |
                    PC3             PC4
             172.16.0.3/16   172.16.0.4/16



            
