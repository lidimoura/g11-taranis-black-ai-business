# G11 — Taranis Black | AI for Business

MVP privado para o Challenge G11, estruturado para a Rota Zero e a Rota 3 — RH e People Analytics.

## Objetivo

Analisar a base sintética de colaboradores e clima da Taranis Black, identificar sinais de turnover e apoiar a proposta de um simulador de treinamento de lideranças baseado no modelo SBI (Situação, Comportamento e Impacto).

## Arquitetura conceitual

- **Bronze:** arquivos originais do kit de dados, mantidos fora deste repositório.
- **Prata:** leitura, padronização, validação de tipos e criação de indicadores derivados no notebook.
- **Ouro:** tabelas agregadas, achados executivos, hipóteses e gráficos para o relatório.

Esta é uma arquitetura conceitual de MVP. Não representa um data warehouse produtivo.

## Como executar no Google Colab

1. Abra `notebooks/01_people_analytics_mvp.ipynb` no Google Colab.
2. Execute as células em ordem.
3. Faça upload de `04_Base_Colaboradores_People_Analytics.xlsx` quando solicitado.
4. Revise os números, gráficos e ressalvas metodológicas.
5. Use os resultados no Google Docs oficial do Challenge.

## Escopo

Inclui diagnóstico de People Analytics, validações básicas, hipóteses, AI Canvas resumido, priorização e métricas do simulador SBI. Não inclui decisão automatizada de RH, dados pessoais no repositório, deploy produtivo ou integração com sistemas reais.
