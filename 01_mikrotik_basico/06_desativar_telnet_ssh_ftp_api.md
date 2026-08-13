---
title: Mikrotik Basico - Desativar Telnet SSH FTP API
tags:
  - rede/mikrotik
---

# 6 - Desativar - TELNET, SSH, FTP, API

```bash
/ip service set telnet disabled=yes
/ip service set ftp disabled=yes
/ip service set www port=8080
/ip service set ssh disabled=yes
/ip service set api disabled=yes
/ip service set api-ssl disabled=yes

```