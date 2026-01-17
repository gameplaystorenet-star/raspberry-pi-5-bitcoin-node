# 06 - Bitcoin Core como Serviço (systemd)

Este documento descreve como configurar o Bitcoin Core (`bitcoind`) para
rodar como um serviço do sistema, iniciando automaticamente no boot
e reiniciando em caso de falhas.

---

## 🎯 Objetivo

- Executar o Bitcoin Core em segundo plano
- Iniciar automaticamente no boot
- Garantir estabilidade 24/7
- Facilitar logs e manutenção

---

## 👤 Criar usuário dedicado (bitcoin)

Execute no Raspberry Pi:

```bash
sudo adduser --disabled-password --gecos "" bitcoin
