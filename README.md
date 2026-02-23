# Windows Optimizer Pro V5.2 ULTRA PRO

[![PowerShell 5.1+](https://img.shields.io/badge/PowerShell-5.1%2B-blue)](https://github.com/PowerShell/PowerShell)
[![PowerShell 7+](https://img.shields.io/badge/PowerShell-7.x-brightgreen)](https://github.com/PowerShell/PowerShell)
[![MIT License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)
[![Windows 10/11](https://img.shields.io/badge/Windows-10%20%7C%2011-0078D6)](https://microsoft.com)
[![Linux](https://img.shields.io/badge/Linux-PowerShell_7%2B-FCC624)](https://github.com/PowerShell/PowerShell)

Otimizador de sistema profissional com IA, interface grafica moderna e versao CLI para Linux.

## Funcionalidades

### Windows (GUI)
- **IA com 12 metricas reais**: RAM, CPU, Disco, PageFile, Telemetria, Startup, Windows Update, HDD, Temp files, Tasks terceiros, Driver GPU, Game Mode
- **Top 5 processos em tempo real**: RAM e CPU, atualiza a cada 5 segundos
- **Edge Deep Clean**: para o Edge e limpa Cache, Code Cache, GPUCache, ShaderCache, Service Worker, WebStorage
- **TRIM Avancado**: usa `Get-Volume` — mais robusto que `Optimize-Volume` por letra
- **SoftwareDistribution/Download**: limpo na limpeza profunda (pacotes ja aplicados)
- **Comparativo Antes/Depois**: snapshot de Score, RAM e Temp antes e depois de otimizar
- **Historico do Score**: ultimas 10 medicoes com data/hora
- **PageFile inteligente**: formula Microsoft (1x RAM inicial, 3x RAM maximo)
- **Scheduled Tasks terceiros**: lista e analisa tarefas externas ao Windows
- **Network Adapter Advanced**: RSS, LSOv2, Interrupt Moderation, Flow Control
- **Plano de energia**: nunca alterado — mantido padrao Windows

### Linux (CLI)
- Analise IA: CPU load, RAM, disco, swap, atualizacoes, servicos com falha
- Limpeza: /tmp, /var/tmp, apt/dnf/pacman cache, ~/.cache, thumbnails
- Navegadores: Chrome, Chromium, Firefox, Brave, Edge (Linux)
- Rede: benchmark DNS, latencia, interfaces
- Relatorio TXT exportavel
- Modo auto (`-Auto`) para uso em scripts/cron

## Uso

### Windows
```
Clique direito em EXECUTAR_OTIMIZADOR_V5_2_ULTRA.bat
Selecione "Executar como Administrador"
```

### Linux
```bash
# Instalar PowerShell 7+
# Ubuntu/Debian:
sudo apt-get install -y powershell

# Executar (interativo)
sudo pwsh linux_optimizer.ps1

# Modo automatico (sem prompts)
sudo pwsh linux_optimizer.ps1 -Auto

# So relatorio
pwsh linux_optimizer.ps1 -Report
```

## Seguranca

| O que NAO e tocado | Motivo |
|---|---|
| Servicos Windows criticos | Windows nao inicia sem eles |
| `System32/` e `SysWOW64/` | Arquivos do OS |
| `WinSxS/` | Gerenciado apenas pelo DISM |
| Plano de energia | Padrao Windows e o recomendado |
| Drivers em `C:\Windows\System32\drivers\` | Nunca deletar |
| Senhas e dados pessoais do navegador | Edge Deep Clean nunca toca |

## Ratings V5.2
- **Seguranca: 8.5/10** — nunca toca servicos criticos
- **Funcionalidade: 8.5/10** — Edge Deep, TRIM avancado, SoftwareDistribution, Linux CLI
- **IA: 6.5/10** — heuristica avancada com 12 metricas reais

## Licenca
MIT License — use, modifique e distribua livremente.
