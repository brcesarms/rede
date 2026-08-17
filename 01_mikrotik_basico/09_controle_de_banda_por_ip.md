---
title: "Mikrotik Básico: Controle de Banda por IP"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/qos
---

# 📊 Mikrotik Básico: Controle de Banda por IP

> [!info] Limitação de largura de banda (Upload/Download) para IPs específicos usando as Simple Queues do Mikrotik.

---

```bash
/queue simple add max-limit=768k/768k name=Roteador-WIFI target=192.168.10.30/32

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Priorização de Sites e Serviços](08_priorizar_sites_e_serviços.md) — Configuração de priorização de tráfego de sites e serviços.
