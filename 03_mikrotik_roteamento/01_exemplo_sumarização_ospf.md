---
title: "Mikrotik Roteamento: Exemplo de Sumarização OSPF"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/roteamento
  - rede/ospf
---

# 🛣️ Mikrotik Roteamento: Exemplo de Sumarização OSPF

> [!info] Exemplo de sumarização de redes no OSPF para otimização do tamanho da tabela de rotas e desempenho do roteamento.

---

```bash
/routing ospf area 
add area-id=0.0.0.1 name=PPPoE_Clientes

```

```bash
/routing ospf area range 
add area=PPPoE_Clientes range=10.250.2.0/24

```

```bash
/routing ospf network 
add area=PPPoE_Clientes comment=PPPoE_Clientes network=10.250.2.0/24

```


## 🔗 Notas Relacionadas
- [Rede: Guia Principal de Referência de Conhecimento](../README.md) — Índice geral de notas de infraestrutura de redes.
- [Roteamento de IPs Internos: Planejamento de Sub-redes](../roteamento/roteamento_ips_internos.md) — Planejamento estruturado de sub-redes e IPs internos.
