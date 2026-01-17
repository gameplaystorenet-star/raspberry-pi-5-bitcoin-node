# 07 - Monitoramento e Manutenção do Nó Bitcoin

Este documento descreve como monitorar, verificar a integridade e realizar
manutenção segura de um nó Bitcoin Core rodando em um Raspberry Pi 5.

---

## 🎯 Objetivos

- Acompanhar o status de sincronização do blockchain
- Monitorar saúde e desempenho do serviço
- Analisar logs do Bitcoin Core
- Executar manutenção sem risco de corrupção de dados
- Garantir operação estável 24/7

---

## 🔎 Verificar status do serviço

Execute no Raspberry Pi:

```bash
systemctl status bitcoind
