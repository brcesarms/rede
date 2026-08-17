---
title: "Mikrotik Básico: Alterando Usuário e Senha de Administração"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/seguranca
---

# 🔑 Mikrotik Básico: Alterando Usuário e Senha de Administração

> [!info] Procedimento essencial de segurança para alteração das credenciais padrão de administração no Mikrotik RouterOS.

---

## ⚙️ Para adicionar
```bash
/user add group=full name=bruno password=linuxap

```
   
 
## ⚙️ Para remover
```bash
/user remove admin

```


## 🔗 Notas Relacionadas
- [Mikrotik Básico: Guia de Referência de Configurações](README_mikrotik_basico.md) — Índice de tópicos de Mikrotik Básico.
- [Mikrotik Básico: Desativando Serviços Inseguros](06_desativar_telnet_ssh_ftp_api.md) — Desativação de serviços administrativos inseguros no Mikrotik.
- [Mikrotik Firewall: Guia de Segurança e Proteção Essencial](../02_mikrotik_firewall/01_básico_para_proteger_seu_mikrotik.md) — Regras fundamentais de firewall para proteção do RouterOS.
