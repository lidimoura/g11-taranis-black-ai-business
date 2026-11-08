# Arquitetura MVP — Taranis Black Intelligence Hub

## Bronze

Fonte original: `04_Base_Colaboradores_People_Analytics.xlsx`, fornecida no kit sintético do Challenge G11. O arquivo original não é versionado neste repositório.

## Prata

O notebook lê as abas `Base_Colaboradores`, `Pesquisa_Clima_Qualitativa` e `KPIs_Gerais_RH`; remove linhas de cabeçalho duplicadas; padroniza tipos; calcula status, departamento, desligamento e permanência; e verifica contagens e valores ausentes.

## Ouro

O notebook produz tabelas agregadas por departamento, indicadores de turnover, médias de eNPS e clima, contagem de desligamentos até 90 dias, gráficos e hipóteses de negócio. Os resultados devem ser revisados antes de serem apresentados como evidência executiva.

## Governança

A análise é agregada. Comentários qualitativos não devem ser usados para identificar indivíduos. O simulador SBI é uma ferramenta de treinamento e não pode decidir contratação, promoção, desligamento ou punição.
