---
title: "Mikrotik Básico: Bloqueio de Sites e Serviços"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/seguranca
  - rede/firewall
---

# 🔑 Mikrotik Básico: Bloqueio de Sites e Serviços

> [!info] Bloqueio de acessos a sites ou serviços de rede específicos usando regras de filtro e listas de endereços no Mikrotik.

---

```bash
/ip firewall address-list add address=192.168.10.30 list="Fora do bloqueio do Youtube"

```
 
```bash
/ip firewall filter add action=drop chain=forward comment="Bloqueio Youtube" content=youtube src-address=192.168.10.0/27 src-address-list="!Fora do bloqueio do Youtube"

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Priorização de Sites e Serviços](08_priorizar_sites_e_serviços.md) — Configuração de priorização de tráfego de sites e serviços.
- [Mikrotik Firewall: Guia de Segurança e Proteção Essencial](../02_mikrotik_firewall/01_básico_para_proteger_seu_mikrotik.md) — Regras fundamentais de firewall para proteção do RouterOS.
