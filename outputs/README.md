# Evidências Analíticas Agregadas — Outputs (Fase 2)

Este diretório armazena **exclusivamente resultados e gráficos agregados e anonimizados** da camada Ouro do notebook `notebooks/01_people_analytics_mvp.ipynb`, gerados a partir da base sintética educacional da Taranis Black (`04_Base_Colaboradores_People_Analytics.xlsx`).

## Governança e Privacidade (LGPD / Privacy by Design)

- A planilha bruta (`04_Base_Colaboradores_People_Analytics.xlsx`) permanece fora do repositório (protegida via `.gitignore`).
- Na camada Prata, as colunas de identificação individual (`Nome`) e remuneração (`Salário Mensal (R$)`) são descartadas antes de qualquer agregação.
- Nenhum gráfico ou tabela exibe nomes, e-mails, salários ou comentários individuais identificáveis.

## Arquivos Gerados

1. `01_turnover_por_departamento.png`: Taxa de turnover observado por departamento comparada à média corporativa da Taranis Black (22,9% na base detalhada / 22,8% na aba de KPIs).
2. `02_clima_dimensoes_agregadas.png`: Médias agregadas (escala 1 a 5) das três dimensões da Pesquisa Qualitativa de Clima (`n = 14`): Carga de Trabalho (`2,07`), Ferramentas/Processos (`2,43`) e Liderança Direta (`3,07`).
3. `03_motivos_desligamento_agregados.png`: Distribuição percentual agregada dos motivos reportados nas entrevistas de saída dos desligados (`n = 64`).
