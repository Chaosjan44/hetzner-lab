1. Primary IP will be NAT to our pfSense.
    - our pfSense will have the following ports forwared:
        - 80 -> docker host
        - 443  -> docker host



# IPs in general
- Public IPs
    - Primary IPv4 `46.4.52.118` *vmbr50*
        - GW `46.4.52.65`
        - Netmask `255.255.255.192`
    - Secondary IPv4 `46.4.52.106` *vmbr51*
        - GW `46.4.52.65`
        - Netmask `255.255.255.192`

- IPs between host and pfSense
    - Host IPv4 `10.255.255.253`
    - pfSense WAN IPv4 `10.255.255.254`
    - Netmask `255.255.255.252`

- IPs inside pfSense *vmbr0*
    - pfSense LAN IPv4 `172.30.0.1`
    - GW `172.30.0.1`
    - Netmask `255.255.255.0`
    - Netbird GW `172.30.0.3`
    - Docker `172.30.0.10`

- DMZ (not yet used) *vmbr5*