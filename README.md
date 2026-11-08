# G11 — Taranis Black | AI for Business

**Versão:** MVP de entrega  
**Status:** em execução controlada pela CEO  
**Classificação:** projeto privado de preparação e portfólio  
**Responsável:** Lídi Moura  
**Empresa simulada:** Taranis Black  
**Rota:** Rota Zero + Rota 3 — IA para RH e People Analytics  
**Data de abertura:** 2026-11-08

## Regra de autoridade e aprovação

Lídi Moura é a autoridade máxima sobre escopo, narrativa, decisão de rota, conteúdo enviado, publicação, links e entrega. O Antigravity atua como executor técnico e documental: analisa, implementa, testa e propõe. Ele não publica, envia, altera permissões externas ou toma decisões estratégicas sem revisão da CEO.

O trabalho é executado por fases. Ao final de cada fase, o Antigravity deve apresentar artefatos, evidências, riscos, decisões pendentes e recomendações. A próxima fase só começa após revisão da CEO.

## Regra de privacidade

Os dados da Taranis Black são sintéticos para fins educacionais. Ainda assim, o projeto deve aplicar minimização, anonimização e controle de acesso. Não versionar planilhas originais, nomes, e-mails, salários, comentários identificáveis, credenciais, tokens, JWTs, senhas, arquivos `.env` ou dumps.

## Objetivo do projeto

Construir uma proposta executiva de IA responsável para a Taranis Black, usando a Rota Zero e a Rota 3 do Challenge G11. A solução prioritária é um simulador de treinamento de lideranças baseado no modelo SBI — Situação, Comportamento e Impacto — para prática segura de conversas difíceis.

## Resultado que precisa ser entregue

A entrega oficial será um Google Docs preenchido com o template do Challenge, compartilhado como visualização por link. O documento deve conter o diagnóstico, AI Canvas, três casos de uso, Matriz Esforço × Impacto, Política de IA Responsável, plano de métricas, gestão de mudanças, simulador SBI, evidências, links e limitações.

O GitHub privado, Colab, Canva e showcase são artefatos de apoio e portfólio. Nenhum deles substitui o Google Docs oficial.

## Descoberta e fontes

### Fontes prioritárias

- `Challenge G11 - Taranis Black.txt`: enunciado e critérios.
- `00_INDICE_E_GUIA_DO_KIT_DE_DADOS.md`: mapa do kit.
- `04_Base_Colaboradores_People_Analytics.xlsx`: base da Rota 3.
- Cursos e NotebookLM: material de estudo e apoio metodológico.
- Projetos de Show My Projects: referência de portfólio, não guia obrigatório.
- Documentação oficial de ferramentas: fonte para funções, limites e permissões atuais.

### Hierarquia de decisão

Instruções explícitas da CEO; requisitos do Challenge; governança e segurança do Hub OS; arquivos do projeto; evidências calculadas; documentação oficial de ferramentas; materiais de estudo; hipóteses.

## Proposta de solução

### Caso prioritário

Simulador de treinamento de liderança com persona sintética de colaborador desafiador, prática de feedback SBI, rubrica de avaliação, segunda tentativa, feedback construtivo e supervisão humana.

### Casos complementares

1. Análise assistida de clima e temas recorrentes.
2. Onboarding inteligente para os primeiros 90 dias.

### Fora do escopo do MVP

Data Warehouse produtivo, Power BI completo, automação real de RH, integração com sistemas, deploy, autenticação, publicação pública e incorporação permanente de métodos ao hub-os-guIA.

## Arquitetura analítica conceitual

- **Bronze:** arquivos originais mantidos fora do GitHub.
- **Prata:** limpeza, padronização, validação e anonimização no Colab.
- **Ouro:** tabelas agregadas, gráficos, hipóteses e indicadores executivos.

A arquitetura é conceitual e serve ao MVP. Não representa infraestrutura produtiva.

## Artefatos

- `notebooks/01_people_analytics_mvp.ipynb`: análise reproduzível no Colab.
- `docs/MVP_ARCHITECTURE.md`: arquitetura conceitual.
- `docs/AI_CANVAS_R0_R3.md`: AI Canvas resumido.
- `ANTIGRAVITY_COMMAND_MVP_G11.md`: comando executor por fases.
- `DELIVERY_QA_CHECKLIST_G11.md`: evidências e QA da entrega.
- `reports/`: relatório, política e plano de métricas.
- `simulator/`: prompt e documentação do simulador SBI.
- `showcase/`: demonstração visual local, sem publicação automática.
- `outputs/`: somente imagens e resultados agregados, quando autorizados.

## Fluxo operacional por fases

### Fase 0 — alinhamento

Confirmar rota, requisitos, fontes, fora de escopo e formato oficial. Saída: plano de trabalho e decisões pendentes.

### Fase 1 — diagnóstico

Executar o notebook, validar indicadores e registrar limitações. Saída: tabelas, gráficos e achados agregados.

### Fase 2 — Rota Zero

Produzir AI Canvas, três casos de uso, Matriz Esforço × Impacto, métricas, gestão de mudanças e política responsável.

### Fase 3 — Rota 3

Criar e testar o simulador SBI com cenário fictício, rubrica e segunda tentativa.

### Fase 4 — documentação

Montar relatório executivo e organizar prompts, links, prints e referências.

### Fase 5 — showcase

Criar página ou materiais visuais apenas depois de a entrega oficial estar completa.

### Fase 6 — QA e handoff

Executar o checklist, revisar o Google Docs e entregar à CEO um pacote pronto para envio manual na Alura.

## Critérios de aceite

- Todos os requisitos da Rota Zero aparecem no Google Docs.
- A missão obrigatória da Rota 3 aparece com evidência do simulador.
- A análise usa a base de People Analytics sem expor dados individuais.
- Hipóteses não são apresentadas como causalidade.
- A política inclui LGPD, vieses, supervisão humana e limites de uso.
- Os prompts usados estão documentados.
- Os prints estão legíveis e contextualizados.
- Os links funcionam em modo visualização.
- Nenhum segredo ou arquivo bruto foi versionado.

## Registro STAR — rascunho

- **Situation:** Taranis Black cresceu rapidamente, mas enfrenta sinais de fragilidade em turnover, liderança e experiência inicial.
- **Task:** propor uma fundação de IA responsável e um caso de uso prioritário para RH.
- **Action:** analisar a base sintética, estruturar AI Canvas, priorizar casos e criar simulador SBI.
- **Result:** MVP documentado e demonstrável; resultado de negócio ainda não medido.

## Métricas

As métricas de negócio e adoção ficam documentadas em `reports/03_plano_metricas_e_gestao_mudanca.md`. O MVP não afirma redução de turnover; apenas define como medir viabilidade, aprendizagem, adoção e resultados futuros.

## DEVLOG

Toda decisão relevante deve registrar data, evidência, alternativas, risco, recomendação, aprovação necessária e próximo passo. O DEVLOG deve ser atualizado ao final de cada fase.

## Governança de publicação

Não publicar, enviar para a Alura, compartilhar externamente, mudar permissões do Drive, publicar o showcase ou alterar infraestrutura sem revisão explícita da CEO. O repositório permanece privado enquanto o projeto estiver em validação.
