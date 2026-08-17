---
title: "Mikrotik Básico: Configuração de DMZ (Demilitarized Zone)"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/firewall
  - rede/dmz
---

# ↕️ Mikrotik Básico: Configuração de DMZ (Demilitarized Zone)

> [!info] Definição de uma zona desmilitarizada no Mikrotik para expor de forma direta um host interno para acessos da internet.

---

```bash
/ip firewall nat add action=dst-nat chain=dstnat dst-address=186.219.242.3 dst-port=!8291 protocol=tcp to-addresses=192.168.1.4 to-ports=0-65535

```
 
 
## ⚙️ ou
 
```bash
/ip firewall nat add action=dst-nat chain=dstnat dst-port=!8291 protocol=tcp to-addresses=192.168.1.4 to-ports=0-65535

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Configuração de NAT (Network Address Translation)](03_nat.md) — Configuração de mascaramento de rede (NAT) no RouterOS.
- [Mikrotik Básico: Redirecionamento de Portas (Port Forwarding)](05_redirecionamento_porta.md) — Redirecionamento de portas externas para serviços internos (DST-NAT).
