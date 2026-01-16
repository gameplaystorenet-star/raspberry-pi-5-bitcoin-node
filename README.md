# Raspberry Pi 5 Bitcoin Node (Step-by-Step)

Projeto completo e documentado para configurar um **nó Bitcoin** em um **Raspberry Pi 5**, com acesso remoto seguro via **Tailscale**, usando **Debian GNU/Linux 13 (Trixie)**.

Este guia foi desenvolvido para ser reproduzível, estável e acessível mesmo através de **dados móveis (4G/5G)**.

---

## 📦 Hardware Utilizado

- Raspberry Pi 5 (8 GB ou 16 GB recomendado)
- Armazenamento NVMe ou SSD (1 TB ou mais recomendado)
- Fonte oficial ou equivalente
- Conexão à internet (Ethernet ou Wi-Fi)

---

## 🧠 Sistema Operacional

- **Debian GNU/Linux 13 (Trixie)**
- Kernel Raspberry Pi (`rpi-6.12+`)
- Arquitetura: `aarch64`

Verificação:
```bash
lsb_release -a
uname -a
