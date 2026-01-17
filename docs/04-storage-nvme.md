# 04 – Armazenamento NVMe (Bitcoin Node)

Este documento descreve a preparação, identificação e montagem do armazenamento NVMe
para uso com um Raspberry Pi 5 rodando um nó Bitcoin.

⚠️ **Importante**:  
Até este ponto, o sistema ainda roda no **microSD**.  
O NVMe será usado **exclusivamente para dados do Bitcoin**.

---

## 🎯 Objetivo

- Utilizar NVMe para alto desempenho e durabilidade
- Evitar uso intensivo do microSD
- Garantir estabilidade para sincronização do Bitcoin Core

---

## 🧰 Hardware Utilizado

- Raspberry Pi 5
- Case ou HAT compatível com NVMe (ex: PCIe / M.2)
- SSD NVMe (1 TB ou maior recomendado)
- Fonte oficial Raspberry Pi 5 (5V / 5A)

---

## 🔍 Identificação do NVMe

Com o NVMe conectado ao Raspberry Pi, execute:

```bash
lsblk
