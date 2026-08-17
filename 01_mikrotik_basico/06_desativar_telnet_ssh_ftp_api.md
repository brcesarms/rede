---
title: "Mikrotik Básico: Desativando Serviços Inseguros"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/seguranca
---

# 🔑 Mikrotik Básico: Desativando Serviços Inseguros

> [!info] Proteção do RouterOS através do bloqueio ou desativação de portas de serviços administrativos vulneráveis ou não utilizados.

---

```bash
/ip service set telnet disabled=yes
/ip service set ftp disabled=yes
/ip service set www port=8080
/ip service set ssh disabled=yes
/ip service set api disabled=yes
/ip service set api-ssl disabled=yes

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Alterando Usuário e Senha de Administração](02_alterando_usuário_senha.md) — Procedimento de alteração de usuário e senha de administração.
- [Mikrotik Firewall: Guia de Segurança e Proteção Essencial](../02_mikrotik_firewall/01_básico_para_proteger_seu_mikrotik.md) — Regras fundamentais de firewall para proteção do RouterOS.
