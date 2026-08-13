---
title: Mikrotik Basico - NAT
tags:
  - rede/mikrotik
---

# 3 - NAT

```bash
/ip firewall nat add action=masquerade chain=srcnat comment=Full-masquerade

```
 
## ou

```bash
/ip firewall nat add action=masquerade chain=srcnat comment=Mascaramento out-interface=ether1

```