# 🛡️ Blue Team Lab – Wazuh SOC Environment

Mini laboratório Blue Team utilizando :contentReference[oaicite:0]{index=0} e Windows para simulação e monitoramento de eventos de segurança em ambiente controlado.

---

## 🎯 Objetivo

Este laboratório tem como objetivo praticar conceitos fundamentais de Blue Team e SOC, incluindo:

- Monitoramento e análise de logs
- Detecção de falhas de autenticação no Windows
- Monitoramento de execução de PowerShell
- Auditoria de eventos de firewall
- Criação de regras básicas de detecção no Wazuh

---

## 🧰 Tecnologias Utilizadas

- Wazuh (SIEM / XDR)
- Windows 10 (Endpoint)
- Ubuntu Server (Wazuh Manager)
- VirtualBox (Ambiente virtualizado)
- PowerShell
- Windows Event Logs

---

## 🏗️ Arquitetura do Ambiente


Windows Client (Agent)
│
▼
Wazuh Agent (Coleta de logs)
│
▼
Wazuh Manager (Análise e correlação)
│
▼
Alertas de segurança (JSON / Dashboard)


---

## 📊 Eventos Monitorados

O laboratório foca na geração e detecção dos seguintes eventos:

### 🔐 Autenticação Windows
- Event ID **4624** → Login bem-sucedido
- Event ID **4625** → Falha de autenticação

### ⚙️ PowerShell
- Execução de comandos suspeitos
- Histórico de comandos

### 🔥 Firewall Windows
- Alterações em regras de entrada/saída
- Bloqueios e liberações de tráfego

### 👤 Usuários locais
- Criação de novos usuários
- Alterações em contas locais

---

## 🧠 Objetivo Técnico

- Entender funcionamento de um SIEM na prática
- Simular cenários reais de ataque e defesa
- Trabalhar com logs estruturados
- Criar base para estudos em SOC / Blue Team

---

## 🚀 Objetivo Futuro

Evolução do laboratório com:

- Sysmon para telemetria avançada
- Active Directory (cenário corporativo)
- Regras customizadas no Wazuh
- Detecção baseada em comportamento
- Integração com MITRE ATT&CK

---

## 📌 Observação

Este é um ambiente totalmente controlado e utilizado exclusivamente para fins educacionais e de aprendizado em segurança da informação.
