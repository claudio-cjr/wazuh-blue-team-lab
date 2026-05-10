# 📝 Notes — Security Event Analysis

Esta pasta contém anotações e análises realizadas durante os testes do laboratório Blue Team utilizando Wazuh, Sysmon e Windows Event Logs.

Os arquivos documentam cenários simulados de segurança, incluindo:

* tentativas de brute force
* execução suspeita de PowerShell
* enumeração de contas locais
* análise de eventos Sysmon
* correlação com MITRE ATT&CK

---

# 🎯 Objetivo

O objetivo desta seção é registrar o processo de investigação e análise de eventos de segurança gerados no ambiente de laboratório, simulando atividades comuns em operações de SOC (Security Operations Center).

Cada caso contém:

* hipótese inicial
* evidências coletadas
* eventos observados
* severidade
* análise técnica
* conclusão

---

# 📂 Casos Documentados

| Caso                     | Descrição                                             |
| ------------------------ | ----------------------------------------------------- |
| brute-force.md           | Simulação de múltiplas falhas de autenticação Windows |
| powershell-suspicious.md | Monitoramento de atividade suspeita via PowerShell    |
| account-discovery.md     | Enumeração de contas locais utilizando `net.exe`      |

---

# 🧠 Conceitos Praticados

* Investigação de logs
* Correlação de eventos
* Telemetria Windows
* Monitoramento com Sysmon
* Integração SIEM
* MITRE ATT&CK
* Troubleshooting de eventos
* Análise básica de incidentes

---

# 📌 Observação

Todos os cenários foram executados em ambiente controlado e possuem finalidade exclusivamente educacional e de aprendizado em segurança da informação.

