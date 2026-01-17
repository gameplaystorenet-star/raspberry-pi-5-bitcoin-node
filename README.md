![Release](https://img.shields.io/github/v/release/gameplaystorenet-star/raspberry-pi-5-bitcoin-node)
![Status](https://img.shields.io/badge/status-stable-brightgreen)
![License](https://img.shields.io/github/license/gameplaystorenet-star/raspberry-pi-5-bitcoin-node)
![Platform](https://img.shields.io/badge/platform-Raspberry%20Pi%205-red)
# Raspberry Pi 5 Bitcoin Full Node

Este projeto documenta, passo a passo, a instalação, configuração e operação
de um **nó completo Bitcoin Core** utilizando um **Raspberry Pi 5** com
armazenamento **NVMe**, foco em **segurança, estabilidade e privacidade**.
---

## 🚀 Quick Start (Resumo rápido)

Para usuários que já conhecem Linux e querem subir o nó rapidamente.

```bash
# 1. Atualizar o sistema
sudo apt update && sudo apt upgrade -y

# 2. Preparar o NVMe (exemplo)
sudo mkfs.ext4 /dev/nvme0n1
sudo mkdir -p /mnt/bitcoin
sudo mount /dev/nvme0n1 /mnt/bitcoin

# 3. Instalar Bitcoin Core
sudo apt install bitcoind bitcoin-cli -y

# 4. Ativar o serviço
sudo systemctl enable bitcoind
sudo systemctl start bitcoind

1. [01-installation.md](docs/01-installation.md)  
   Instalação do sistema operacional

2. [02-network-and-remote-access.md](docs/02-network-and-remote-access.md)  
   Rede, SSH e acesso remoto

3. [03-security.md](docs/03-security.md)  
   Segurança básica do sistema

4. [04-storage-nvme.md](docs/04-storage-nvme.md)  
   Preparação e uso do NVMe

5. [05-bitcoin-core.md](docs/05-bitcoin-core.md)  
   Instalação e configuração do Bitcoin Core

6. [06-bitcoind-systemd.md](docs/06-bitcoind-systemd.md)  
   Bitcoin Core como serviço (systemd)

7. [07-monitoring-and-maintenance.md](docs/07-monitoring-and-maintenance.md)  
   Monitoramento e manutenção

8. [08-backups-and-recovery.md](docs/08-backups-and-recovery.md)  
   Backup e recuperação

9. [09-tor.md](docs/09-tor.md)  
   Bitcoin Core com Tor (privacidade)


## 🎯 Objetivos do Projeto

- Rodar um nó Bitcoin completo (full node)
- Utilizar NVMe para alto desempenho e durabilidade
- Operar 24/7 de forma estável
- Garantir segurança básica e boas práticas
- Permitir operação opcional via Tor (privacidade)
- Servir como referência para outros usuários

---

## 🧰 Hardware Recomendado

- Raspberry Pi 5 (8 GB ou 16 GB)
- SSD NVMe (1 TB ou maior)
- Case ou HAT compatível com NVMe (ex: PCIe / M.2)
- Fonte oficial Raspberry Pi 5 (5V / 5A)
- Cartão microSD (apenas para o sistema)

---

## 📚 Estrutura da Documentação

Siga os arquivos **na ordem** abaixo:
 

---

## ⚠️ Avisos Importantes

- A blockchain pode ser baixada novamente
- **Carteiras e configurações NÃO**
- Faça backups regulares
- Use Tor apenas se entender as implicações

---

## 📜 Licença

Este projeto é disponibilizado para fins educacionais.
Use por sua conta e risco.
---

## ▶️ Como usar este repositório

Siga os arquivos da pasta `docs/` em ordem numérica, do 01 ao 09.

---

## ⚠️ Aviso Importante

Projeto educacional. Você é responsável pela operação do seu nó.
