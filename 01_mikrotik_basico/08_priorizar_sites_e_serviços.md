---
title: "Mikrotik Básico: Priorização de Sites e Serviços"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/qos
---

# 📊 Mikrotik Básico: Priorização de Sites e Serviços

> [!info] Otimização de tráfego de rede e QoS no Mikrotik para priorizar serviços sensíveis ou sites cruciais.

---

```bash
/ip firewall mangle 
add action=add-dst-to-address-list address-list=Lista-IPTV address-list-timeout=1d chain=prerouting content=tv5.cs10.tv src-address=192.168.11.0/24 
add action=mark-connection chain=prerouting dst-address-list=Lista-IPTV new-connection-mark=tv-conexoes passthrough=yes 
add action=mark-packet chain=prerouting connection-mark=tv-conexoes new-packet-mark=tv-pacotes passthrough=yes

```

```bash
/queue tree 
add limit-at=3M max-limit=3M name=IPTV packet-mark=tv-pacotes parent=global priority=1

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Controle de Banda por IP](09_controle_de_banda_por_ip.md) — Limitação de largura de banda para IPs específicos usando Simple Queues.
- [Mikrotik Básico: Bloqueio de Sites e Serviços](07_bloqueio_sites_serviços.md) — Bloqueio de acessos a sites ou serviços de rede específicos.
