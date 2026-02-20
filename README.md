# 🛡️ Homelab SOC - Fundação Sobrevivi

Este repositório documenta a infraestrutura do meu laboratório de segurança, focado em hospedar o banco de dados da **Fundação Sobrevivi**. O projeto serve como base prática para as certificações **Linux Essentials** e **AZ-900**.

---

## 🏗️ Inventário de Hardware (The Beast)
* **Processador:** Intel Core i3-3220 (3.30 GHz, 3ª Geração)
* **Memória RAM:** 4GB DDR3
* **Armazenamento:** HD Mecânico 150GB SATA
* **Sistema Operacional:** Ubuntu Server 20.04 LTS

## 🌐 Infraestrutura de Rede & Troubleshooting
O ambiente foi reestruturado para eliminar problemas de **Double NAT**, garantindo uma comunicação direta e estável.

### Ativos de Rede:
* **Roteador Secundário:** TP-Link TL-WR840N
* **Configuração:** Modo Access Point (Bridge) com DHCP desativado.

### Gerenciamento de Endereçamento (Hardening):
Para evitar conflitos de IP, o escopo DHCP do modem principal foi limitado, isolando uma faixa exclusiva para os ativos do lab:
* **Faixa DHCP Comum:** 192.168.2.2 até 192.168.2.250
* **IP Roteador TP-Link (Gerência):** `192.168.2.251`
* **IP Servidor Ubuntu (Fixo):** `192.168.2.252`
* **Gateway:** `192.168.2.1`

---

## 🛠️ Implementações Realizadas (Dia 2)
- [x] **Troubleshooting de Rede:** Identificação e resolução de NAT duplo e conflitos de rota.
- [x] **Networking:** Configuração de IP estático via Netplan na interface `enp2s0`.
- [x] **Acesso Remoto:** Instalação e validação do OpenSSH Server.
- [x] **Segurança de Host:** Ativação do Firewall (UFW) com permissão restrita para a porta 22 (SSH).

---
**Analista Responsável:** Welesson de Oliveira de Sousa  
**Objetivo Profissional:** Analista de SOC (G4F)
