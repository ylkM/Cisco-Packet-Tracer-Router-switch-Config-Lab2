# Cisco Basic LAN – Router & Switch Configuration



## Topology

```text
                         172.16.0.0/16
                              |
                       R1 G0/0: 172.16.0.254
                              |
                         SW1 G0/1
                              |
              +---------------+---------------+
              |                               |
          SW1 Fa0/1                       SW1 Fa0/2
              |                               |
          PC1 .1                           PC2 .2

                         SW1 G0/2
                              |
                         SW2 G0/1
                          /       \
                    Fa0/1         Fa0/2
                      |             |
                    PC3 .3        PC4 .4
```

## IP Addressing

| Device | Interface | IP Address | Subnet Mask | Gateway |
|---|---|---|---|---|
| R1 | G0/0 | 172.16.0.254 | 255.255.0.0 | — |
| PC1 | Fa0 | 172.16.0.1 | 255.255.0.0 | 172.16.0.254 |
| PC2 | Fa0 | 172.16.0.2 | 255.255.0.0 | 172.16.0.254 |
| PC3 | Fa0 | 172.16.0.3 | 255.255.0.0 | 172.16.0.254 |
| PC4 | Fa0 | 172.16.0.4 | 255.255.0.0 | 172.16.0.254 |

## Configuration Tasks Covered

1. Hostnames configured for R1, SW1, and SW2.
2. IP addressing configured for R1 and all PCs.
3. Speed and duplex manually configured on links between networking devices.
4. Interface descriptions added.
5. Unused interfaces disabled with `shutdown`.

## Files

- `R1-config.txt` – R1 CLI configuration
- `SW1-config.txt` – SW1 CLI configuration
- `SW2-config.txt` – SW2 CLI configuration
- `PC-IP-addressing.txt` – PC addressing instructions
- `README.md` – Project documentation

## Verification

After configuration, test connectivity from each PC:

```text
ping 172.16.0.254
ping 172.16.0.1
ping 172.16.0.2
ping 172.16.0.3
ping 172.16.0.4
```

On Cisco devices:

```text
show ip interface brief
show interfaces status
show running-config
```

