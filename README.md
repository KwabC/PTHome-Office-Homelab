# Packet Tracer Basic LAN Setup Homelab

This homelab simulates a small office network with three wired computers, one printer, and a wireless laptop using DHCP to test connectivity.

**Packet Tracer version used:** 9.0.1

## Topology 
<img width="911" height="490" alt="Home Office LAN" src="https://github.com/user-attachments/assets/62806687-780b-4131-80f0-36d63792d5ef" />


## IP Addressing
| Device | Interface | IP Address | Subnet Mask | Area |
|--------|-----------|------------|--------------|------|
| R0 | Gi0/0 | 192.168.1.1 | 255.255.255.0 | 0 |
| WR0 | Gi0/0 | 192.168.2.2 | 255.255.255.0 | 0 |
| PC1 | FE0 | 192.168.1.4 | 255.255.255.0 | 0 |
| PC2 | FE0 | 192.168.1.3 | 255.255.255.0 | 0 |
| PC3 | FE0 | 192.168.1.2 | 255.255.255.0 | 0 |
| LAP0 | WIR0 | 192.168.2.100 | 255.255.255.0 | 0 |
| PTR0 | FE0 | 192.168.1.101 | 255.255.255.0  | 0 |
| SW0 | FE0 | N/A | N/A | 0 |

## Key Commands/Notes
- Connected All PCs to SW0 using straight-through cables
- Connected R0 and PTR0 to SW0 using a straight-through cable
- Connected WR0 to R0 using a crossover-cable
- Used 'ip dhcp pool LAN' to set up a dhcp pool for wired devices on the 192.168.1.0/24 network
- Used 'ip dhcp pool WLAN' to set up a dhcp pool for wireless devices on the 192.168.2.0/24 network
- Set up a static ip address for PTR0
- Pinged the routers and printer to test stable connectivity

## Files
[Router0_config.txt](https://github.com/user-attachments/files/33068336/Router0_config.txt)


