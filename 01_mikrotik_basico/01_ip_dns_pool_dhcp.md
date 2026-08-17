---
title: "Mikrotik Básico: Configuração de IP, DNS, Pool e DHCP"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/dhcp
  - rede/dns
---

# 🔌 Mikrotik Básico: Configuração de IP, DNS, Pool e DHCP

> [!info] Configurações fundamentais do RouterOS para definição de endereçamento IP, servidores DNS, pool de endereços e DHCP Server.

---

## 🔌 IP
```bash
/ip address add address=192.168.10.1/24 interface=LAN network=192.168.10.0

```
   
## 🔌 DNS
```bash
/ip dns set servers=1.0.0.1,8.8.4.4,208.67.220.220

```
   
## 🔌 POOL
```bash
/ip pool add name=dhcp_pool0 ranges=192.168.10.2-192.168.10.254

```
 
## 🔌 DHCP SERVER
```bash
/ip dhcp-server add address-pool=dhcp_pool0 disabled=no interface=LAN name=dhcp1

```
 
```bash
/ip dhcp-server network add address=192.168.10.0/24 dns-server=8.8.4.8,1.0.0.1 gateway=192.168.10.1

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Configuração de Servidor DNS Local](10_servidor_dns_mikrotik.md) — Configuração avançada do servidor DNS local no Mikrotik.
- [Mikrotik Básico: Configuração de NAT (Network Address Translation)](03_nat.md) — Configuração de mascaramento de rede (NAT) para saída à internet.
