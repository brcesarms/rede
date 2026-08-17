---
title: "Mikrotik Básico: Redirecionamento de Portas (Port Forwarding)"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/firewall
  - rede/nat
---

# ↕️ Mikrotik Básico: Redirecionamento de Portas (Port Forwarding)

> [!info] Configurações de DST-NAT para redirecionamento de portas específicas no RouterOS, permitindo acessos externos a servidores locais.

---

```bash
/ip firewall nat add action=dst-nat chain=dstnat comment="rota vnc CAIXA1" dst-port=39803 protocol=tcp to-addresses=192.168.10.3 to-ports=5900

```
 
## ⚙️ ou

```bash
/ip firewall nat add action=dst-nat chain=dstnat comment="CAMERAS SERVER" dst-address=177.11.164.10 to-addresses=192.168.2.3

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Configuração de NAT (Network Address Translation)](03_nat.md) — Configuração de mascaramento de rede (NAT) no RouterOS.
- [Mikrotik Básico: Configuração de DMZ (Demilitarized Zone)](04_dmz.md) — Configuração de zona desmilitarizada (DMZ) no Mikrotik.
