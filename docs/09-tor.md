# 09 - Bitcoin Core com Tor (Privacidade e Anonimato)

Este documento descreve como configurar o Bitcoin Core para operar através da rede Tor
em um Raspberry Pi 5, aumentando a privacidade, ocultando o IP público e permitindo
operações como nó Tor (opcionalmente onion-only).

---

## 🎯 Objetivos

- Ocultar o endereço IP real do nó Bitcoin
- Aumentar privacidade na rede Bitcoin
- Permitir conexões via Tor (`.onion`)
- Reduzir exposição a monitoramento de rede
- Preparar o nó para uso remoto seguro

---

## ⚠️ Avisos Importantes

- Tor **não deixa o nó mais rápido**, apenas mais privado
- A sincronização inicial pode ser **mais lenta**
- É recomendado usar **NVMe** (como já configurado)
- Tor é altamente recomendado para nós públicos ou acessados remotamente

---

## 📦 Instalação do Tor

No Raspberry Pi, execute:

```bash
sudo apt update
sudo apt install tor -y
