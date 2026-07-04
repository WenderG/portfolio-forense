# 02 - Análise de Memória Volátil (Memory Forensics)

**Status:** Concluído  
**Caso:** Captura de Memória RAM em Máquina Virtual  
**Data:** 04 de Julho de 2026

## Objetivo

Demonstrar a captura e análise de memória RAM usando Volatility 3 para extrair processos, conexões de rede, linhas de comando e outros artefatos voláteis.

## Ferramentas Utilizadas

- **Magnet RAM Capture** — Captura da memória
- **Volatility 3.2.28.0** — Análise forense da memória

## Metodologia

1. Criação de Máquina Virtual Windows
2. Captura da memória RAM enquanto o sistema executava aplicações normais
3. Análise com Volatility 3 (plugins principais)

## Resultados Principais

- **Sistema identificado**: Windows 10 (Build 19041)
- **Número de Processos**: Diversos processos ativos (System, smss, csrss, svchost, explorer, msedge, OneDrive, etc.)
- **Conexões de rede**: Múltiplas conexões TCP/UDP detectadas
- **Artefatos recuperados**: Linhas de comando, árvore de processos, serviços em execução

## Arquivos Gerados

- `info.txt` — Informações do sistema
- `pslist.txt` e `pstree.txt` — Lista de processos
- `netscan.txt` — Conexões de rede
- `cmdline.txt` — Linhas de comando

## Evidências

**Exemplos de saída:**
- [Informações do Sistema](./resultados/info.txt)
- [Lista de Processos](./resultados/pslist.txt)
- [Árvore de Processos](./resultados/pstree.txt)
- [Conexões de Rede](./resultados/netscan.txt)

## Conclusão

A análise de memória volátil é essencial para identificar processos ocultos, malware em execução e artefatos que não ficam registrados em disco. Este projeto demonstra o uso prático do Volatility 3 em um cenário controlado.

**Aprendizado:** A combinação de captura + análise permite recuperar informações críticas em investigações de incidentes.

---

**Última atualização:** 04 de Julho de 2026
