---
title: "Roteamento de IPs Internos: Planejamento de Sub-redes"
date_created: 2026-08-17
tags:
  - rede/roteamento
---

# 🔌 Roteamento de IPs Internos: Planejamento de Sub-redes

> [!info] Estudo e planejamento de faixas de IPs privados de sub-redes internas para evitar colisões e otimizar rotas.

---

Veja aqui quais são os IPs que devem ser utilizados numa rede internet
```bash
10.0.0.0/8 (do IP 10.0.0.1 até 10.255.255.255)
172.16.0.0/12 (do IP 172.16.0.1 até 172.31.255.255)
192.168.0.0/16 (do IP 192.168.0.1 até 192.168.255.255)

```

Não utilize nenhuma outra faixa de IPs em sua rede interna que não sejam listados acima. Podem ser utilizados também IPs públicos fornecidos pela operadora ou os pertencentes ao ASN do provedor.

## 🔌 Memorizando barramento IPs
```bash
/24 - 256
/25 - 128
/26 - 64
/27 - 32
/28 - 16

```


## 🔗 Notas Relacionadas
- [Rede: Guia Principal de Referência de Conhecimento](../README.md) — Índice geral de notas de infraestrutura de redes.
- [Mikrotik Roteamento: Exemplo de Sumarização OSPF](../03_mikrotik_roteamento/01_exemplo_sumarização_ospf.md) — Exemplo prático de sumarização de redes no protocolo OSPF.
