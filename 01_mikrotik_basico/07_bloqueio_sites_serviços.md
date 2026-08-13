---
title: Mikrotik Basico - Bloqueio Sites e Servicos
tags:
  - rede/mikrotik
---

# 7 - Bloqueio: SITES e SERVIÇOS

```bash
/ip firewall address-list add address=192.168.10.30 list="Fora do bloqueio do Youtube"

```
 
```bash
/ip firewall filter add action=drop chain=forward comment="Bloqueio Youtube" content=youtube src-address=192.168.10.0/27 src-address-list="!Fora do bloqueio do Youtube"

```