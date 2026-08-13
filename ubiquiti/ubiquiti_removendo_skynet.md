---
nome: Removendo vírus Skynet
tags:
  - rede/ubiquiti
---

# Removendo SkyNet

PuTTY
```bash
rm /etc/persistent/rc.poststart rm -rf /etc/persistent/.skynet cfgmtd -w -p /etc/  reboot

```

