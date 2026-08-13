---
title: " DNS AdGuard Home"
tags:
  - rede/dns
  - rede/firewall
sources:
  - https://youtu.be/r5J9gGQVXM0?si=vuPeV20ZMzYEHX-E
  - https://youtu.be/B2V_8M9cjYw?si=tBXXPEFZeNUq6Qwa
---

Os endereços IP públicos do AdGuard DNS variam conforme o nível de filtragem desejado:

- **Padrão** (bloqueia anúncios e rastreadores): IPv4 **94.140.14.14** e **94.140.15.15**; IPv6 **2a10:50c0::ad1:ff** e **2a10:50c0::ad2:ff**. 
- **Proteção Familiar** (bloqueia conteúdo adulto e ativa busca segura): IPv4 **94.140.14.15** e **94.140.15.16**; IPv6 **2a10:50c0::bad1:ff** e **2a10:50c0::bad2:ff**. 
- **Sem Filtragem** (apenas resolução de DNS): IPv4 **94.140.14.140** e **94.140.14.141**; IPv6 **2a10:50c0::1:ff** e **2a10:50c0::2:ff**. 

Para dispositivos Android 9+, é possível usar o **DNS Privado** configurando o nome de host **dns.adguard.com**.