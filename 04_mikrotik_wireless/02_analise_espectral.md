---
title: "Mikrotik Wireless: Análise Espectral de Radiofrequência"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/wireless
---

# 📶 Mikrotik Wireless: Análise Espectral de Radiofrequência

> [!info] Uso das ferramentas de Spectral Scan e History do RouterOS para identificar fontes de interferência de RF.

---

```bash
interface wireless spectral-history 0 range=5500-5800

```

```bash
interface wireless spectral-scan 0 range=5500-5800

```


## 🔗 Notas Relacionadas
- [Rede: Guia Principal de Referência de Conhecimento](../README.md) — Índice geral de notas de infraestrutura de redes.
- [Tutorial: Varredura e Seleção do Melhor Canal Wi-Fi no Linux com nmcli](../tutorial-nmcli-wifi.md) — Guia de seleção de canais Wi-Fi com nmcli no Linux.
