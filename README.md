# Packet Tracer Basic LAN Setup Homelab

This homelab simulates a small office network with three wired computers, one printer, and a wireless laptop using DHCP to test connectivity.

**Packet Tracer version used:** 9.0.1

## Topology 
<img width="907" height="467" alt="diagram png" src="https://github.com/user-attachments/assets/5a9a1837-eea9-4d33-b38a-32dacff65962" />

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
- Used ip dhcp pool LAN for wired devices
- Used ip dhcp pool WLAN for wireless devices
- Pinged the routers and printer to ensure stable connectivity

## Files


