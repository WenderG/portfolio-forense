# 02 - Análise de Memória Volátil (Memory Forensics)

**Status:** Concluído  
**Caso:** Captura de Memória RAM em Máquina Virtual  
**Data:** 04 de Julho de 2026

## Objetivo

Demonstrar a captura e análise de memória RAM para extração de processos, conexões de rede, linhas de comando e artefatos voláteis.

## Ferramentas Utilizadas

- **Magnet RAM Capture** — Captura da memória
- **Volatility 3.2.28.0** — Análise forense da memória

## Metodologia

1. Criação de Máquina Virtual Windows
2. Captura da memória RAM enquanto executava aplicações normais
3. Análise com Volatility 3 (plugins principais)

## Resultados Principais

- **Sistema identificado**: Windows 10 (Build 19041)
- **Número de Processos**: Muitos em execução (incluindo svchost, explorer, msedge, OneDrive, etc.)
- **Conexões de rede**: Detectadas várias conexões ativas (TCP/UDP)
- **Artefatos recuperados**: Linhas de comando, processos em árvore, serviços, etc.
- Arquivos de saída gerados: `info.txt`, `pslist.txt`, `pstree.txt`, `netscan.txt`, `cmdline.txt`

## Evidências

- [Captura da Memória](./memoria/memoria-captura-01.raw) (não versionado)
- [Exemplo de saída - Processos](./resultados/pslist.txt)
- [Exemplo de saída - Árvore de Processos](./resultados/pstree.txt)
- [Exemplo de saída - Rede](./resultados/netscan.txt)

## Conclusão

Este projeto demonstra a importância da análise de memória volátil para identificar processos ocultos, conexões suspeitas e artefatos que não ficam registrados em disco. É uma técnica essencial em investigações de incidentes e malware.

**Aprendizado:** Volatility 3 é extremamente poderoso para extrair informações em tempo real da RAM.

---

**Última atualização:** 04 de Julho de 2026