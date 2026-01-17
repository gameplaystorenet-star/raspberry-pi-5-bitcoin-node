# 03 – Segurança Básica do Sistema

Este documento descreve as configurações mínimas de segurança recomendadas
para operar um Raspberry Pi 5 como nó Bitcoin, priorizando simplicidade,
estabilidade e acesso remoto seguro.

---

## 🎯 Objetivos

- Evitar acessos não autorizados
- Manter o sistema simples e auditável
- Garantir acesso remoto seguro via SSH e Tailscale
- Minimizar superfície de ataque

---

## 🔐 Segurança do SSH

### Verificar status do SSH
Execute no Raspberry Pi:

```bash
systemctl status ssh
