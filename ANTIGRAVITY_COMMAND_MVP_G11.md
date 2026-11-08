# Comando mestre para o Antigravity — MVP G11

Copie o bloco abaixo como uma única instrução no Antigravity, com o repositório privado `lidimoura/g11-taranis-black-ai-business` aberto.

---

Você é o agente executor técnico e documental do projeto privado **G11 — Taranis Black | AI for Business**. O objetivo é concluir hoje um MVP enxuto, demonstrável e alinhado ao enunciado do Challenge G11, para a **Rota Zero + Rota 3 — IA para RH e People Analytics**. Não amplie o escopo e não crie infraestrutura produtiva.

## Protocolo de execução controlada pela CEO

Execute uma fase por vez. Ao concluir cada fase, PARE e entregue um checkpoint com: (a) arquivos criados ou alterados; (b) evidências produzidas; (c) decisões tomadas; (d) alternativas consideradas; (e) riscos e limitações; (f) QA executado; (g) decisões que exigem aprovação da CEO; (h) recomendação do próximo passo. Não avance para a fase seguinte sem a revisão explícita da CEO.

Use o README do repositório como contrato operacional e siga o template do Hub OS guIA: Identificação, Regra de privacidade, Objetivo, Descoberta, Proposta de solução, Entrega e validação, Artefatos, Critérios de aceite, STAR e DEVLOG.

Fases obrigatórias: Fase 0 — alinhamento e inventário; Fase 1 — diagnóstico e QA dos dados; Fase 2 — Rota Zero; Fase 3 — simulador SBI da Rota 3; Fase 4 — documentação e evidências; Fase 5 — showcase somente se a entrega oficial estiver completa; Fase 6 — QA final e handoff. Se houver pouco tempo, priorize Fases 0 a 4 e deixe o showcase para depois.

## Contexto obrigatório

A Taranis Black é uma empresa brasileira de ergonomia corporativa, com 280 colaboradores, faturamento anual de R$ 48 milhões e crescimento acelerado. O desafio exige uma proposta executiva de IA para a CEO.

A Rota Zero exige obrigatoriamente:

1. Aplicar o AI Canvas;
2. Mapear três casos de uso de IA;
3. Construir a Matriz Esforço × Impacto;
4. Criar plano de métricas;
5. Propor gestão de mudanças;
6. Redigir Política Corporativa de IA Responsável com LGPD, mitigação de vieses e supervisão humana.

A Rota 3 exige obrigatoriamente criar um simulador de treinamento de liderança: um agente que assume a persona de uma pessoa colaboradora desafiadora para que gestores pratiquem o modelo de feedback SBI — Situação, Comportamento e Impacto — em ambiente seguro.

## Fontes autorizadas

Use os arquivos compartilhados do projeto, especialmente:

- `Challenge G11 - Taranis Black.txt` — requisitos e formato;
- `00_INDICE_E_GUIA_DO_KIT_DE_DADOS.md` — mapa das fontes;
- `04_Base_Colaboradores_People_Analytics.xlsx` — base sintética da Rota 3;
- `00_BASE_CHALLENGE_R0_R3.md` — estrutura inicial já produzida;
- `docs/MVP_ARCHITECTURE.md`;
- `docs/AI_CANVAS_R0_R3.md`;
- `notebooks/01_people_analytics_mvp.ipynb`.

Os projetos de Show My Projects são somente referência de portfólio. Não trate-os como regras ou fonte de verdade. Os notebooks do NotebookLM são materiais de estudo; não copie transcrições integrais nem incorpore métodos ao hub-os-guIA.

## Entregáveis a criar ou completar no repositório

Crie os seguintes arquivos, sem incluir dados brutos, nomes de pessoas, e-mails, credenciais, tokens, JWTs ou arquivos `.env`:

1. `reports/01_relatorio_executivo_g11.md`
2. `reports/02_politica_ia_responsavel_taranis_black.md`
3. `reports/03_plano_metricas_e_gestao_mudanca.md`
4. `simulator/README.md`
5. `simulator/prompt_simulador_sbi.md`
6. `showcase/index.html`
7. `showcase/README.md`
8. `outputs/README.md`

Mantenha e melhore o notebook existente. Se gerar gráficos, salve somente imagens agregadas e anonimizadas em `outputs/`. Nunca salve a planilha original no repositório.

## Conteúdo obrigatório do relatório executivo

O relatório deve ser escrito para a CEO, em linguagem clara e objetiva, e conter:

- resumo executivo;
- contexto de negócio;
- pergunta de negócio;
- fontes e limitações;
- arquitetura analítica conceitual Bronze → Prata → Ouro, explicitando que é apenas uma arquitetura de MVP;
- diagnóstico agregado de People Analytics;
- AI Canvas dos três casos de uso;
- Matriz Esforço × Impacto;
- justificativa da escolha do simulador SBI;
- plano de métricas;
- plano de gestão de mudanças;
- política de IA responsável resumida;
- roadmap em fases;
- riscos, controles e próximos passos;
- checklist de evidências para o Google Docs oficial.

Use a planilha como evidência quantitativa principal. Não misture a narrativa do enunciado com a planilha sem registrar a diferença: o enunciado menciona aproximadamente 24% de turnover nos primeiros 90 dias, enquanto a aba consolidada da planilha informa 23,4%. Trate isso como arredondamento ou divergência a reconciliar.

Não declare causalidade. Use expressões como “os dados sugerem”, “foi observado” e “hipótese a validar”.

## Conteúdo obrigatório do simulador SBI

O prompt deve criar uma pessoa colaboradora fictícia e desafiadora, sem usar dados reais. O fluxo deve:

1. apresentar um cenário;
2. solicitar o feedback da pessoa gestora;
3. responder como a persona;
4. avaliar a resposta conforme Situação, Comportamento e Impacto;
5. avaliar especificidade, tom, escuta e próximo passo;
6. oferecer feedback construtivo;
7. permitir uma segunda tentativa;
8. encerrar com plano de ação.

O agente deve declarar que é uma simulação de treinamento. Deve proibir o uso para contratação, promoção, desligamento, punição ou avaliação oficial. Deve solicitar intervenção humana quando houver risco de assédio, discriminação, crise, saúde mental ou conflito grave.

## Conteúdo obrigatório da Política de IA Responsável

Incluir:

- usos permitidos;
- usos proibidos;
- dados que nunca devem ser enviados a ferramentas externas;
- anonimização e minimização;
- supervisão humana;
- proibição de decisões automatizadas de RH;
- mitigação de vieses;
- revisão e contestação humana;
- controle de acesso por função;
- registro de finalidade, ferramenta e responsável;
- revisão periódica da política.

## Showcase

Crie uma página HTML estática simples, elegante e responsiva, sem frameworks externos obrigatórios, que apresente:

- título do projeto;
- problema de negócio;
- números agregados da base;
- três casos de uso;
- destaque do simulador SBI;
- fluxo do simulador;
- política de IA responsável;
- roadmap;
- nota de que os dados são sintéticos e a solução é um MVP acadêmico.

Não publique a página. Apenas deixe o arquivo pronto para demonstração local e futura publicação autorizada.

## Regras de segurança e qualidade

- Não hardcode credenciais.
- Não incluir `.env`.
- Não publicar ou fazer deploy.
- Não usar dados de clientes reais.
- Não adicionar nomes, e-mails ou identificadores pessoais ao relatório ou showcase.
- Não criar decisões automatizadas sobre pessoas.
- Não afirmar que o MVP reduziu turnover.
- Não fazer correlações causais sem evidência.
- Não apagar arquivos existentes sem necessidade.
- Executar validação de Markdown, JSON do notebook e HTML.
- Conferir que o repositório não contém arquivos `.xlsx`, `.csv` ou segredos.
- Atualizar o README com instruções de execução e lista de entregáveis.

## Critério de conclusão

Ao finalizar, mostre:

1. lista dos arquivos criados ou alterados;
2. validações executadas;
3. principais indicadores usados;
4. limitações conhecidas;
5. instruções de como abrir o notebook no Colab;
6. instruções de como usar o prompt do simulador;
7. o que ainda precisa ser copiado para o Google Docs oficial.

Não gaste tempo com Power BI, Canva, banco de dados, pipeline produtivo, autenticação, deploy ou integração real. Esses itens ficam no roadmap pós-challenge.
