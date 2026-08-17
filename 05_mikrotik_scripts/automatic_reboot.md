---
title: "Mikrotik Scripts: Reinicialização Automática Programada"
date_created: 2026-08-17
tags:
  - rede/mikrotik
  - rede/scripts
---

# 💻 Mikrotik Scripts: Reinicialização Automática Programada

> [!info] Script e agendador para automatizar o reboot periódico do roteador, otimizando o uso de memória do RouterOS.

---

## 🔌 Script
```bash
system script

```

```bash
add dont-require-permissions=no name=automatic_reboot owner=suporte policy=\
    ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon source=\
    "system reboot\r\
    \ny\r\
    \n"

```

## ⚙️ Scheduler
```bash
system scheduler

```

```bash
add interval=1d name=schedule_automatic_reboot on-event=\
    schedule_automatic_reboot policy=\
    ftp,reboot,read,write,policy,test,password,sniff,sensitive,romon \
    start-date=feb/25/2024 start-time=04:00:00

```


## 🔗 Notas Relacionadas
- [Rede: Guia Principal de Referência de Conhecimento](../README.md) — Índice geral de notas de infraestrutura de redes.
- [Mikrotik Básico: Script de Configuração SXT (2016)](../01_mikrotik_basico/13_script_sxt_2016.md) — Script básico de provisionamento de antena SXT.
