# Checklist de Entrega — Challenge G11 (Status Final QA Auditado)

## Regra de entrega oficial

A entrega da Alura aceita o **link do Google Docs preenchido**. Os demais materiais estão vinculados dentro do documento por hyperlinks e por gráficos/prints incorporados nativamente. O notebook Colab, o simulador SBI, o showcase e o GitHub funcionam como evidências complementares auditáveis.

## Mapa de artefatos

| Artefato | Onde criar/salvar | Deve aparecer no Google Docs? | Evidência recomendada |
|---|---|---:|---|
| Relatório final | Google Docs | Sim, é a entrega principal | Link do documento |
| AI Canvas | Google Docs + `docs/AI_CANVAS_R0_R3.md` | Sim | Tabelas e seção completa |
| Três casos de uso | Google Docs | Sim | AI Canvas + Classificação de IA |
| Matriz Esforço × Impacto | Google Docs + `outputs/04_matriz_esforco_impacto.png` | Sim | Imagem legível e explicação |
| Política de IA Responsável | Google Docs + `reports/02_politica_ia_responsavel_taranis_black.md` | Sim | Seção textual completa (Pode / Não Pode) |
| Notebook de análise | Google Colab (`notebooks/01_people_analytics_mvp.ipynb`) | Sim | Link e prints das tabelas/gráficos |
| Base de dados | Apenas ambiente local/Colab | Não anexar ao GitHub | Resultados e gráficos 100% anonimizados |
| Simulador SBI | `simulator/prompt_simulador_sbi.md` + `simulator/README.md` | Sim | Link, prompt completo e sessão de teste |
| Plano de métricas e mudança | `reports/03_plano_metricas_e_gestao_mudanca.md` | Sim | Tabelas de métricas e 4 fases de mudança |
| Showcase | `showcase/index.html` | Opcional / Complementar | Página HTML responsiva versionada |

## Requisitos obrigatórios da Rota Zero

- [x] Contexto da Taranis Black explicado para a CEO (incluindo visão sistêmica dos processos legados).
- [x] Pergunta ou problema de negócio definido.
- [x] AI Canvas aplicado.
- [x] Três casos de uso mapeados (com classificação por tipo de IA: Generativa, Tradicional e Preditiva).
- [x] Matriz Esforço × Impacto preenchida (tabela + gráfico 2×2 incorporado).
- [x] Caso prioritário justificado (Simulador SBI atacando 40,6% das causas de desligamento).
- [x] Plano de métricas criado (Adoção, Aprendizagem SBI, Horas Economizadas, Viabilidade/ROI e KPIs).
- [x] Plano inicial de gestão de mudanças criado (4 fases considerando o esgotamento das lideranças).
- [x] Política Corporativa de IA Responsável criada (formato prático Pode / Não Pode).
- [x] LGPD, privacidade, anonimização (k-anonymity e remoção de Nome/Salário na Prata) e supervisão humana abordadas.
- [x] Comitê de Governança e rituais de auditoria (mensal, trimestral, semestral) definidos.
- [x] Riscos e limitações declarados.

## Requisitos obrigatórios da Rota 3

- [x] Diagnóstico usa a base sintética de People Analytics (`n = 280` e `n = 14` no clima).
- [x] Turnover, primeiros 90 dias, eNPS, liderança, ferramentas/processos e carga de trabalho foram considerados.
- [x] Simulador de liderança criado.
- [x] 3 Personas de colaboradores desafiadores criadas com dados 100% fictícios (Lucas Andrade — Comercial B2B; Marina Costa — Suporte <90d; Rafael Mendes — Operações/Logística).
- [x] Modelo SBI explicado: Situação, Comportamento e Impacto.
- [x] Simulação testada com cenário completo.
- [x] Segunda tentativa e ciclo de melhoria demonstrados (evolução de 2,0/10 na 1ª tentativa para 10,0/10 na 2ª tentativa).
- [x] Feedback do agente estruturado por rubrica de 5 critérios (0 a 10 pontos).
- [x] Avaliação da eficácia do simulador e melhorias v2.0 do prompt documentadas.
- [x] Uso do simulador limitado a treinamento ("Academia Segura de Liderança").
- [x] Proibição explícita de decisões automatizadas de contratação, promoção, desligamento ou punição (Art. 20 LGPD).

## QA final antes de enviar

- [x] O documento abre sem login em janela anônima (`Shared: true` como Leitor/Viewer).
- [x] Todos os links internos e do repositório GitHub (`reports/02_politica_ia_responsavel_taranis_black.md`, `simulator/prompt_simulador_sbi.md`, `docs/AI_CANVAS_R0_R3.md`, `notebooks/01_people_analytics_mvp.ipynb`, `showcase/index.html`) respondem HTTP 200.
- [x] O Google Docs está em modo visualização para qualquer pessoa com o link.
- [x] O nome da ferramenta e o objetivo aparecem junto de cada evidência.
- [x] Os gráficos (`01` a `04`) estão legíveis e incorporados nativamente no Google Docs e no repositório (`outputs/`).
- [x] Nenhum print ou tabela mostra nome real, e-mail de colaborador, salário ou dado identificável.
- [x] Nenhum arquivo `.env`, token, senha ou credencial foi incluído.
- [x] O relatório não afirma causalidade sem evidência.
- [x] A diferença entre 24% no enunciado, 23,4% na aba de KPIs e 13 casos ≤90d (20,3%) na base detalhada está registrada como ressalva.
- [x] O simulador é apresentado como treinamento, não como avaliação oficial.
- [x] A Política de IA Responsável está completa.
- [x] O notebook Colab está acessível e executável.
- [x] A planilha original `.xlsx` não está no repositório GitHub.
