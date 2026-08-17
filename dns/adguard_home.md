---
title: "DNS: Guia Completo do AdGuard Home"
date_created: 2026-08-17
tags:
  - rede/dns
  - rede/seguranca
---

# 🔌 DNS: Guia Completo do AdGuard Home

> [!info] Instalação e configuração do AdGuard Home como servidor DNS local para filtragem de anúncios e controle parental.

---

Os endereços IP públicos do AdGuard DNS variam conforme o nível de filtragem desejado:

- **Padrão** (bloqueia anúncios e rastreadores): IPv4 **94.140.14.14** e **94.140.15.15**; IPv6 **2a10:50c0::ad1:ff** e **2a10:50c0::ad2:ff**. 
- **Proteção Familiar** (bloqueia conteúdo adulto e ativa busca segura): IPv4 **94.140.14.15** e **94.140.15.16**; IPv6 **2a10:50c0::bad1:ff** e **2a10:50c0::bad2:ff**. 
- **Sem Filtragem** (apenas resolução de DNS): IPv4 **94.140.14.140** e **94.140.14.141**; IPv6 **2a10:50c0::1:ff** e **2a10:50c0::2:ff**. 

Para dispositivos Android 9+, é possível usar o **DNS Privado** configurando o nome de host **dns.adguard.com**.


## 🔗 Notas Relacionadas
- [Rede: Guia Principal de Referência de Conhecimento](../README.md) — Índice geral de notas de infraestrutura de redes.
- [Mikrotik Básico: Configuração de Servidor DNS Local](../01_mikrotik_basico/10_servidor_dns_mikrotik.md) — Configuração básica de DNS local no Mikrotik.
