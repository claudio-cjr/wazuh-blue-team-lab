# Wazuh Blue Team Lab

Mini laboratório Blue Team utilizando Wazuh e Windows para monitoramento de eventos de autenticação, PowerShell e firewall.

## Objetivo

Praticar:
- Monitoramento de logs
- Falhas de login Windows
- Eventos PowerShell
- Firewall
- Criação de regras simples no Wazuh

## Tecnologias

- Wazuh
- Windows 10
- Ubuntu Server
- VirtualBox
- PowerShell
- Windows Event Logs

## Estrutura do ambiente

Wazuh Server → coleta e analisa logs

Windows Client → gera eventos e envia logs

## Eventos monitorados

- Event ID 4624 (login bem-sucedido)
- Event ID 4625 (falha de login)
- Eventos PowerShell
- Alterações de firewall
- Criação de usuários locais

## Objetivo futuro

Expandir o laboratório com:
- Sysmon
- Active Directory
- Detecção avançada
- Regras customizadas
