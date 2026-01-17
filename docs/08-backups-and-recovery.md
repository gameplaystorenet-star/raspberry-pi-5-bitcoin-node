# 08 - Backups e Recuperação do Nó Bitcoin

Este documento descreve as práticas recomendadas de backup e recuperação
para um nó Bitcoin Core rodando em Raspberry Pi 5.

Backups corretos garantem proteção contra falhas de hardware, corrupção
de dados e erros humanos.

---

## 🎯 Objetivos

- Proteger configurações críticas do nó
- Garantir recuperação rápida em caso de falha
- Evitar perda de dados importantes
- Manter integridade operacional do Bitcoin Core

---

## 📁 O que PRECISA ser protegido

### 🔹 Arquivos críticos

- `bitcoin.conf`
- Diretório de dados do Bitcoin (`datadir`)
- `wallet.dat` (SE você usar carteira no nó)
- Scripts personalizados (se existirem)

⚠️ **Importante**:  
A blockchain pode ser baixada novamente.  
**Carteiras e configurações NÃO.**

---

## 🔐 Backup do arquivo de configuração

Execute no Raspberry Pi:

```bash
mkdir -p ~/backups/bitcoin
cp /mnt/bitcoin/bitcoin.conf ~/backups/bitcoin/
