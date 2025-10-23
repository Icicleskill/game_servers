# Docker Network Setup

* Main Subnet - 192.168.50.1/23

* Game Servers - 192.168.50.56 - 192.168.50.75

#

MacVlan docker compose settings to assign a specific IP to a container. 

```
services:
  lgsm:
    networks:
      llamamac:
        ipv4_address: 192.168.50.XX

networks:
  llamamac:
    name: llamamac
    driver: macvlan
    driver_opts:
      parent: enp6s18
    ipam:
      config:
        - subnet: "192.168.50.0/23"
          gateway: "192.168.50.1"
```
#
