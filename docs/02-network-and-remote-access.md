# 02 – Rede e Acesso Remoto Seguro

Este documento descreve a configuração de rede cabeada (Ethernet),
verificação de conectividade e acesso remoto seguro ao Raspberry Pi 5
utilizando SSH e Tailscale, inclusive via dados móveis (4G/5G).

---

## 🌐 Configuração de Rede

### Objetivo
- Utilizar **apenas Ethernet (eth0)**
- Manter **Wi-Fi desativado**
- Garantir rota padrão estável para a internet

---

## 🔍 Verificação das Interfaces de Rede

Execute no Raspberry Pi:

```bash
ip a
---

## 🧭 Verificação da Rota Padrão

Execute no Raspberry Pi:

```bash
ip route
