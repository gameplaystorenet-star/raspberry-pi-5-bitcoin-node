# 05 – Bitcoin Core (Instalação e Configuração)

Este documento descreve a instalação, configuração e inicialização do Bitcoin Core
em um Raspberry Pi 5, utilizando NVMe como diretório de dados.

---

## 🎯 Objetivo

- Instalar o Bitcoin Core de forma oficial
- Utilizar o NVMe como `datadir`
- Operar um nó Bitcoin completo (full node)
- Garantir estabilidade e fácil manutenção

---

## 📦 Atualização do Sistema

Execute no Raspberry Pi:

```bash
sudo apt update && sudo apt upgrade -y
