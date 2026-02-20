# 🛡️ Homelab SOC - Fundação Sobrevivi

Este projeto documenta a infraestrutura do meu laboratório de segurança, focado em hospedar o banco de dados da **Fundação Sobrevivi**.

## 🏗️ Hardware (The Beast)
* **CPU:** Intel Core i3 (3ª Geração)
* **RAM:** 4GB DDR3 (Detectado via `free -h`)
* **Disco:** HD Mecânico 150GB
* **SO:** Ubuntu Server 20.04 LTS

## 🌐 Configurações de Rede (Dia 2)
* **IP Fixo:** 192.168.2.252 (Configurado via Netplan na interface `enp2s0`)
* **Gateway:** 192.168.2.1
* **DNS:** 8.8.8.8 (Google)

## 🛠️ Implementações Realizadas
- [x] Configuração de IP estático para servidor de banco de dados.
- [x] Instalação e ativação do OpenSSH Server para acesso remoto.
- [x] Ativação do Firewall (UFW) com permissão para porta 22.
- [x] Documentação oficial iniciada no GitHub.

**Objetivo:** Transição para Analista de SOC (G4F).
