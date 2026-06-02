# 01 - Recuperação Avançada de Dados em Pendrive

**Caso:** Pendrive Defeituoso (8GB)  
**Data:** 26/05/2026

## Objetivo

Demonstrar o processo completo de **aquisição forense** e **recuperação de dados** em um dispositivo de armazenamento com falha.

## Ferramentas Utilizadas

- **FTK Imager 4.7.3.81** — Aquisição e verificação de imagem (.E01)
- **Autopsy 4.23.1** — Análise e Data Carving

## Metodologia

1. Criação de imagem forense bit-a-bit
2. Verificação de integridade (MD5 + SHA1)
3. Análise com ingest modules no Autopsy
4. Recuperação de arquivos deletados (PhotoRec Carver)

## Evidências do Processo

**Prints do Processo:**
- [Criação da Imagem](./prints/01-ftk-create-image.jpg)
- [Verificação de Hashes](./prints/02-ftk-verify-hash.jpg)
- [Análise no Autopsy](./prints/03-autopsy-analysis.jpg)

## Resultados

- Imagem forense criada com sucesso
- Hashes verificados (Match)
- Processamento de Data Carver iniciado no Autopsy

## Conclusão

Este projeto demonstra o fluxo inicial de uma perícia de recuperação de dados, respeitando a cadeia de custódia e boas práticas forenses.

---

**Última atualização:** 26 de Maio de 2026