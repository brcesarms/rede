---
title: Mikrotik Basico - IP DNS POOL DHCP
tags:
  - rede/mikrotik
  - rede/roteamento
---

# 1 - IP, DNS, POOL e DHCP


## IP
```bash
/ip address add address=192.168.10.1/24 interface=LAN network=192.168.10.0

```
   
## DNS
```bash
/ip dns set servers=1.0.0.1,8.8.4.4,208.67.220.220

```
   
## POOL
```bash
/ip pool add name=dhcp_pool0 ranges=192.168.10.2-192.168.10.254

```
 
## DHCP SERVER
```bash
/ip dhcp-server add address-pool=dhcp_pool0 disabled=no interface=LAN name=dhcp1

```
 
```bash
/ip dhcp-server network add address=192.168.10.0/24 dns-server=8.8.4.8,1.0.0.1 gateway=192.168.10.1

```