---
title: "Ubiquiti: Removendo o Malware Skynet"
date_created: 2026-08-17
tags:
  - rede/ubiquiti
  - rede/seguranca
---

# 🔑 Ubiquiti: Removendo o Malware Skynet

> [!info] Guia de detecção, higienização e remoção de scripts maliciosos e trojans em equipamentos Ubiquiti infectados.

---

PuTTY
```bash
rm /etc/persistent/rc.poststart rm -rf /etc/persistent/.skynet cfgmtd -w -p /etc/  reboot

```


## 🔗 Notas Relacionadas
- [Rede: Guia Principal de Referência de Conhecimento](../README.md) — Índice geral de notas de infraestrutura de redes.
- [Mikrotik Firewall: Guia de Segurança e Proteção Essencial](../02_mikrotik_firewall/01_básico_para_proteger_seu_mikrotik.md) — Proteção essencial e segurança de borda no Mikrotik.
