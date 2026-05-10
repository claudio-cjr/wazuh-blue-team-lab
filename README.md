# 🛡️ Blue Team Lab – Wazuh SOC Environment

Mini laboratório Blue Team utilizando Ubuntu Server e Windows para simulação, coleta e monitoramento de eventos de segurança em ambiente controlado.

---

# 🎯 Objetivo

Este laboratório foi desenvolvido com o objetivo de praticar conceitos fundamentais de Blue Team e SOC (Security Operations Center), incluindo:

* Monitoramento e análise de logs
* Coleta de eventos Windows via Wazuh Agent
* Detecção de atividades suspeitas
* Monitoramento de PowerShell
* Análise de eventos Sysmon
* Correlação de eventos com MITRE ATT&CK
* Troubleshooting de integração SIEM + Endpoint

---

# 🧰 Tecnologias Utilizadas

* Wazuh (SIEM / XDR)
* Sysmon (Sysinternals)
* Windows 10 (Endpoint)
* Ubuntu Server (Wazuh Manager)
* VirtualBox (Ambiente virtualizado)
* PowerShell
* Windows Event Logs
* EventChannel
* MITRE ATT&CK Framework

---

# 🏗️ Arquitetura do Ambiente

```text
Windows Client (Agent)
        │
        ▼
Wazuh Agent (Coleta de logs)
        │
        ▼
Wazuh Manager (Análise e correlação)
        │
        ▼
Dashboard / Alertas / Investigação
```

---

# 📊 Eventos Monitorados

O laboratório foca na geração, coleta e análise de eventos de segurança utilizando Windows Event Logs, Sysmon e Wazuh.

## 🔐 Autenticação Windows

* Event ID 4624 → Login bem-sucedido
* Event ID 4625 → Falha de autenticação

## ⚙️ PowerShell e Execução de Processos

* Execução de comandos PowerShell
* Process Create (Sysmon Event ID 1)
* Criação de arquivos suspeitos (Sysmon Event ID 11)
* Enumeração de contas locais (`net user`)
* Monitoramento de linha de comando

## 🧠 Telemetria e Monitoramento

* Coleta de eventos via EventChannel
* Integração Sysmon + Wazuh
* Monitoramento de atividades administrativas
* Análise de logs no Wazuh Dashboard
* Correlação de eventos com MITRE ATT&CK

## 👤 Usuários Locais

* Consulta e enumeração de contas
* Monitoramento de atividades administrativas
* Detecção de comandos relacionados a usuários locais

---

# 🚨 Detecções Realizadas

Durante os testes foram gerados eventos de segurança monitorados pelo Wazuh, incluindo:

* Execução suspeita de PowerShell
* Criação de arquivos temporários `.ps1`
* Enumeração de contas locais com `net.exe`
* Eventos Sysmon relacionados a criação de processos
* Eventos correlacionados com MITRE ATT&CK

---

# 🧪 Exemplos de Técnicas Monitoradas

| Técnica               | MITRE ATT&CK |
| --------------------- | ------------ |
| Account Discovery     | T1087        |
| PowerShell Execution  | T1059        |
| Ingress Tool Transfer | T1105        |

---

# 🛠️ Troubleshooting e Aprendizados

Durante o desenvolvimento do laboratório foram realizados diversos testes práticos de integração entre Sysmon e Wazuh, incluindo troubleshooting de EventChannel, parsing de eventos e validação de telemetria avançada.

Os testes envolveram:

* configuração manual de XML do Sysmon
* integração de EventChannel no Wazuh Agent
* validação de eventos via Event Viewer
* monitoramento de PowerShell
* análise de eventos Sysmon no Wazuh
* investigação de ingestão de logs no SIEM
* troubleshooting de eventos de telemetria de rede

---

# 🧠 Objetivo Técnico

O laboratório foi desenvolvido para fortalecer conhecimentos práticos em:

* Blue Team
* SOC Analyst
* SIEM
* Análise de logs
* Telemetria Windows
* Investigação de eventos
* Correlação de alertas
* Monitoramento de endpoints

---

# 🚀 Objetivos Futuros

Evolução do laboratório com:

* Active Directory (cenário corporativo)
* Regras customizadas no Wazuh
* Dashboards personalizados
* Detecção baseada em comportamento
* Integração avançada com MITRE ATT&CK
* Simulação de ataques controlados
* Centralização de múltiplos endpoints

---

# 📌 Observação

Este laboratório foi desenvolvido exclusivamente para fins educacionais, aprendizado em segurança da informação e prática de monitoramento defensivo em ambiente controlado.
