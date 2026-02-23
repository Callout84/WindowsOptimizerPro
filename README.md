# Windows Optimizer Pro V5.2

**Otimizador leve, seguro e reversível para Windows 11**

Interface gráfica moderna (WPF dark theme) para limpeza segura, análise de desempenho, otimizações de rede, modo gamer reversível, reparos do sistema e mais.

**Foco principal:**  
- Otimizações leves e nativas do Windows  
- **Nunca** desabilita Defender, Windows Update, Firewall ou serviços críticos  
- Tudo reversível (backups + pontos de restauração)  
- Sem promessas milagrosas — ganhos reais médios de 5–15% dependendo do hardware

MIT License 2026 • Open-source • github.com/[seu-usuario]/windows-optimizer-pro

## ⚠️ Aviso Importante (Leia antes de usar!)
Esta ferramenta faz ajustes **seguros e reversíveis**, mas qualquer mudança no sistema pode ter riscos.  
**Recomendações obrigatórias:**
- Execute **sempre como Administrador**
- Crie um **ponto de restauração manual** antes (ou use o automático da ferramenta)
- Faça backup de dados importantes
- Teste em máquina secundária/VM primeiro se possível
- Resultados variam conforme hardware, drivers e uso

**Não use em servidores de produção ou ambientes corporativos críticos.**

## Funcionalidades Principais
- Análise Heurística com score 0–1000 (12 métricas reais)
- Top processos RAM/CPU em tempo real
- Limpeza segura (temps, caches de drivers/GPU/navegadores, winget update)
- Otimização de rede (DNS inteligente, RSS/LSO, TCP avançado)
- Reparos (DISM + SFC em janela externa)
- Modo Gamer reversível (GPU Scheduling, prioridade multimídia, Nagle OFF)
- Configuração inteligente de pagefile (fórmula Microsoft)
- Histórico de scores + comparativo antes/depois
- Log de ações em %TEMP%

## Como Usar
1. Baixe o repositório (Code → Download ZIP) ou clone:
   ```bash
   git clone https://github.com/[seu-usuario]/windows-optimizer-pro.git
