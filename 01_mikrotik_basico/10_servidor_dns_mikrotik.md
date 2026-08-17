---
title: "Mikrotik Básico: Configuração de Servidor DNS Local"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/dns
---

# 🔌 Mikrotik Básico: Configuração de Servidor DNS Local

> [!info] Configurações de DNS local recursivo e registros estáticos no RouterOS.

---

```bash
/ip firewall filter add action=drop chain=input comment="drop_ataque_dns_udp" dst-port=53 in-interface=pppoe-brunosiqueira protocol=udp
/ip firewall filter add action=drop chain=input comment="drop_ataque_dns_tcp" dst-port=53 in-interface=pppoe-brunosiqueira protocol=tcp

```

```bash
/ip firewall nat add action=redirect chain=dstnat comment="focar_dns_local_udp" dst-port=53 in-interface=!pppoe-brunosiqueira protocol=udp to-ports=53
/ip firewall nat add action=redirect chain=dstnat comment="focar_dns_local_tcp" dst-port=53 in-interface=!pppoe-brunosiqueira protocol=tcp to-ports=53

```
 
 
## ⚙️ ou
 
 
```bash
/ip firewall filter add action=drop chain=input comment=drop_ataque_dns_udp dst-port=53 in-interface=ether1 protocol=udp
/ip firewall filter add action=drop chain=input comment=drop_ataque_dns_tcp dst-port=53 in-interface=ether1 protocol=tcp

```

```bash
/ip firewall nat add action=redirect chain=dstnat comment=focar_dns_local_udp dst-port=53 in-interface=!ether1 protocol=udp to-ports=53
/ip firewall nat add action=redirect chain=dstnat comment=focar_dns_local_tcp dst-port=53 in-interface=!ether1 protocol=tcp to-ports=53

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Configuração de IP, DNS, Pool e DHCP](01_ip_dns_pool_dhcp.md) — Definição de endereçamento IP, DNS, pool e DHCP no Mikrotik.
- [DNS: Guia Completo do AdGuard Home](../dns/adguard_home.md) — Guia de instalação e configuração do servidor DNS AdGuard Home.
