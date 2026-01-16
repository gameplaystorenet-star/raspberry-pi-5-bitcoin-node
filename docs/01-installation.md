# 01 – Instalação do Sistema Base

Este documento descreve a instalação inicial do Raspberry Pi 5, desde o preparo do microSD até o primeiro acesso remoto via rede cabeada.

---

## 🧰 Hardware Utilizado

- Raspberry Pi 5 (8 GB ou 16 GB recomendado)
- Cartão microSD (mínimo 32 GB)
- Fonte oficial Raspberry Pi 5 (5V / 5A)
- Cabo de rede Ethernet
- Armazenamento NVMe ou SSD (será configurado em etapa posterior)

> ⚠️ Nota: neste estágio o sistema roda **apenas no microSD**. O NVMe será configurado depois.

---

## 💿 Sistema Operacional

- Debian GNU/Linux 13 (Trixie)
- Kernel Raspberry Pi (rpi-6.12+)
- Arquitetura: aarch64 (64 bits)

---

## 🔧 Preparação do microSD

1. No computador ou celular, instale o **Raspberry Pi Imager**
2. Selecione:
   - **Raspberry Pi 5**
   - **Raspberry Pi OS (Other) → Debian GNU/Linux 13 (64-bit)**
3. Em configurações avançadas:
   - Defina nome do host (ex: `darkhash-node`)
   - Ative SSH
   - Usuário e senha
   - Desative Wi-Fi (usar apenas Ethernet)
4. Grave a imagem no microSD

---

## 🚀 Primeiro Boot

1. Insira o microSD no Raspberry Pi
2. Conecte o cabo de rede
3. Ligue a fonte
4. Aguarde cerca de 1 minuto

O LED verde ficará piscando durante o boot inicial.

---

## 🌐 Verificação de rede

Após o boot, acesse o Raspberry Pi via terminal (local ou remoto) e execute:

```bash
ip a
