---
title: "Mikrotik Básico: Configuração de NAT (Network Address Translation)"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/firewall
  - rede/nat
---

# ↕️ Mikrotik Básico: Configuração de NAT (Network Address Translation)

> [!info] Configuração de mascaramento de rede (NAT) no RouterOS para permitir que a rede interna acesse a internet de forma segura.

---

```bash
/ip firewall nat add action=masquerade chain=srcnat comment=Full-masquerade

```
 
## ⚙️ ou

```bash
/ip firewall nat add action=masquerade chain=srcnat comment=Mascaramento out-interface=ether1

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Configuração de DMZ (Demilitarized Zone)](04_dmz.md) — Configuração de zona desmilitarizada (DMZ) no Mikrotik.
- [Mikrotik Básico: Redirecionamento de Portas (Port Forwarding)](05_redirecionamento_porta.md) — Redirecionamento de portas externas para serviços internos (DST-NAT).
