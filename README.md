# Raspberry Pi 5 Bitcoin Full Node

Este projeto documenta, passo a passo, a instalação, configuração e operação
de um **nó completo Bitcoin Core** utilizando um **Raspberry Pi 5** com
armazenamento **NVMe**, foco em **segurança, estabilidade e privacidade**.

---

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

1. `01-installation.md`  
   Instalação do sistema operacional

2. `02-network-and-remote-access.md`  
   Rede, SSH e acesso remoto

3. `03-security.md`  
   Segurança básica do sistema

4. `04-storage-nvme.md`  
   Preparação e montagem do NVMe

5. `05-bitcoin-core.md`  
   Instalação e configuração do Bitcoin Core

6. `06-bitcoind-systemd.md`  
   Bitcoin Core como serviço (systemd)

7. `07-monitoring-and-maintenance.md`  
   Monitoramento e manutenção

8. `08-backups-and-recovery.md`  
   Backup e recuperação

9. `09-tor.md`  
   Operação do nó via rede Tor

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
