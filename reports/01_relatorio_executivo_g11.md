# Relatório Executivo Integrado — Taranis Black (Rota Zero + Rota 3)

**Projeto:** Challenge ONE G11 — AI for Business  
**Empresa Simulada:** Taranis Black (Ergonomia Corporativa)  
**Autora / Consultora Executiva:** Lídi Moura (`lidimfc@gmail.com`) | **Turma:** ONE G11  
**Data:** 08/11/2026 | **Classificação:** MVP Executivo com Dados Sintéticos (Conformidade LGPD)  

---

## 1. Resumo Executivo (Para a CEO da Taranis Black — Até 15 Linhas)

**Para:** CEO, Taranis Black | **De:** Lídi Moura, Consultora de IA para Negócios | **Assunto:** Diagnóstico de People Analytics e Plano Executivo de IA Responsável (Rota 0 + Rota 3)

Prezada CEO, o crescimento acelerado da Taranis Black (35% a.a., R$ 48M e 280 colaboradores) superou a maturidade dos nossos processos manuais e de gestão de pessoas, elevando o turnover anual para **22,8%** (22,9% na base detalhada) e o turnover nos primeiros 90 dias para **23,4%** nos KPIs (~24% reportados), com queda do eNPS de **+62 para +28**. Nossa análise em Python/Colab revelou que as saídas se concentram em **Suporte ao Cliente (38,5%)** e **Comercial B2B (30,9%)**, impulsionadas por duas dores combinadas: **comunicação difícil com lideranças recém-promovidas (40,6% dos desligamentos)** e **sobrecarga com tarefas manuais/ERP lento (31,2% geral; 46,2% nos ≤90 dias; nota 2,07/5 em Carga de Trabalho)**. As próprias lideranças intermediárias estão esgotadas pelos sistemas legados e acabam repassando essa pressão às equipes de linha de frente. Recomendamos três iniciativas sob rígida Política de IA Responsável e LGPD: **(1) Prioridade Imediata (Quick Win): Simulador de Liderança no modelo SBI (Situação-Comportamento-Impacto)** com 3 personas sintéticas para treinar conversas difíceis em ambiente seguro; **(2) Análise Assistida de Clima** para monitorar gargalos operacionais de forma anonimizada; e **(3) Onboarding Inteligente 30-60-90 dias**. O MVP já está validado e, sem automatizar decisões de RH, projeta ganhos rápidos em preparo de liderança, horas poupadas de RH e base sólida para retenção sustentável.

---

## 2. Contexto de Negócio, Visão Sistêmica e Pergunta Estratégica

A **Taranis Black** consolidou-se no mercado brasileiro de ergonomia corporativa comercializando cadeiras de alto desempenho (*ErgoPro*), mesas com regulagem elétrica (*SmartDesk*) e cabines acústicas (*Silence*). Contudo, a expansão de 35% ao ano apoiada em fluxos manuais e sistemas legados gerou atritos severos entre áreas:
* **Na Linha de Frente e Operações:** A demora de até 48h para emissão de propostas no ERP, a perda de mais de 40% do tempo comercial em planilhas, os atrasos de 5 dias no fechamento financeiro mensal e a falta de rastreamento de fretes emergenciais (R$ 960k/ano) desaguam diariamente sobre **Comercial B2B** e **Suporte ao Cliente**.
* **No Esgotamento da Liderança:** Coordenadores recém-promovidos, sem treinamento formal de gestão de pessoas e igualmente pressionados por metas e retrabalhos operacionais, evitam conversas individuais estruturadas ou reagem com cobranças ríspidas/coletivas.

**Pergunta de Negócio:** *Como estruturar uma fundação ética de Inteligência Artificial na Taranis Black que capacite imediatamente as lideranças a conduzirem feedbacks construtivos (Modelo SBI) e transforme dados de RH em inteligência preventiva para os primeiros 90 dias, sem violar a LGPD e sem automatizar decisões sobre pessoas?*

---

## 3. Ecossistema de Ferramentas, Transparência e Arquitetura Analítica

### 3.1. Papel Transparente de Cada Recurso Utilizado
1. **Google Docs & Google Drive:** Repositório oficial do enunciado, templates, kit de dados sintéticos, textos exportados das aulas da Alura e documento final de entrega revisado pela CEO.
2. **Google Colab & Python (`pandas`, `matplotlib`, `seaborn`):** Ambiente de execução determinística e auditável para limpeza, anonimização, cálculo de indicadores e geração de gráficos de People Analytics (`notebooks/01_people_analytics_mvp.ipynb`).
3. **Antigravity IDE:** Ferramenta de execução técnica, documental e de QA (enquadrada na categoria *"outra ferramenta"* autorizada pelo enunciado), utilizada sob supervisão da CEO para processar a análise local, estruturar os documentos da Rota 0, redigir e testar o System Prompt do Simulador SBI, gerar gráficos e validar o checklist de qualidade.
4. **Manus AI:** Ambiente inicial de mentoria, coordenação e preparação da estrutura conceitual do projeto e do protocolo de fases, atuando como apoio organizacional sem substituir os entregáveis oficiais.
5. **Hub OS NEXUS & hub-os-guIA (Desenvolvidos por Lídi Moura):**
   - **Hub OS NEXUS:** Arquitetura de governança AI-Native criada por Lídi Moura (*Encontro d'Água Hub — "Reflorestar o Digital"*), aplicada aqui como camada de **segurança, Tolerância Zero a credenciais expostas, Privacy by Design (LGPD), controle de acesso (RBAC) e aprovação humana obrigatória (*Human-in-the-Loop*)**.
   - **hub-os-guIA:** Camada complementar de mentoria técnica e roteamento econômico desenvolvida por Lídi Moura para organizar fontes, separar rigorosamente *fato, hipótese, decisão e evidência*, e estruturar métricas e registro **STAR** para portfólio.
6. **NotebookLM / Acervo de Cursos no Drive:** Fonte de estudo conceitual das trilhas de IA, RH Estratégico, People Analytics e Agentes de IA; como os links web diretos do NotebookLM exigem sessão autenticada de navegador, utilizou-se a contingência oficial prevista no protocolo: leitura dos documentos de cursos exportados na pasta autorizada do Google Drive.
7. **Canva / Showcase HTML:** Camada visual complementar para diagramação executiva do AI Canvas, Matriz Esforço × Impacto e Roadmap.

### 3.2. Arquitetura Analítica Conceitual (Bronze → Prata → Ouro)
* **Camada Bronze (Dados Brutos Isolados):** Planilha `04_Base_Colaboradores_People_Analytics.xlsx` mantida fora do versionamento GitHub (`.gitignore` ativo).
* **Camada Prata (Higienização e Minimização LGPD):** Remoção programática das colunas sensíveis (`Nome` e `Salário Mensal (R$)`), padronização de tipos numéricos e validação de integridade (`280` colaboradores e `14` registros qualitativos de clima sem valores nulos nas colunas críticas).
* **Camada Ouro (Inteligência Agregada):** Tabelas departamentais, taxas de turnover, médias de clima e gráficos anonimizados salvos em `outputs/`. *(Nota: Arquitetura conceitual de MVP, não representando um Data Warehouse produtivo).*

---

## 4. Síntese do Diagnóstico de People Analytics (Rota 3 — Etapa 2 Recomendada)

* **Concentração Departamental Crítica:** Enquanto áreas como Engenharia e P&D (`10,0%` turnover; eNPS `+58`) e Finanças (`13,3%`; eNPS `+32`) apresentam estabilidade relativa, **Suporte ao Cliente (`38,5%` turnover; `32,0%` <90d nos KPIs; eNPS `+08`; absenteísmo de `8,85 dias/ano`)** e **Comercial B2B (`30,9%` turnover; `29,4%` <90d nos KPIs; eNPS `+18`; absenteísmo de `7,16 dias/ano`)** concentram **65,6% de todos os desligamentos da empresa** (42 de 64 saídas).
* **Reconciliação Metodológica Transparente:** O turnover geral é de **22,86% (22,9%)** na Aba 1 (`64/280`) e **22,8%** na Aba 3. Para os primeiros 90 dias, o enunciado cita **~24%**, a Aba 3 reporta **23,4%**, e o filtro estrito `Dias até Desligamento <= 90` na Aba 1 soma **13 casos (20,3% dos desligados / 4,64% da base total)**.
* **Causas Reportadas nas Entrevistas de Saída (`n = 64`):**
  1. *Falta de clareza nas metas e comunicação difícil com a liderança direta:* **40,6% (26 casos)**;
  2. *Sobrecarga com tarefas manuais e sistemas lentos:* **31,2% (20 casos)** — subindo para **46,2%** entre os desligados em até 90 dias;
  3. *Proposta salarial concorrente:* **17,2% (11 casos)**;
  4. *Outros / motivos pessoais:* **10,9% (7 casos)**.
* **Clima Qualitativo (`n = 14`, escala 1–5):** **Carga de Trabalho (`2,07`)**, **Ferramentas/Processos (`2,43`)** e **Liderança (`3,07` geral, caindo para `2,33` em Suporte e Comercial)**.

---

## 5. Síntese da Rota Zero e da Rota 3 (Documentos Completos Vinculados)

1. **Rota Zero — Etapa 1 (AI Canvas, Classificação de IA e Supervisão Humana):** Detalhada integralmente em [`docs/AI_CANVAS_R0_R3.md`](../docs/AI_CANVAS_R0_R3.md).
2. **Rota Zero — Etapa 2 (Matriz Esforço × Impacto, Métricas e Gestão de Mudança):** Detalhada integralmente em [`reports/03_plano_metricas_e_gestao_mudanca.md`](03_plano_metricas_e_gestao_mudanca.md).
3. **Rota Zero — Etapa 3 (Política de IA Responsável, Riscos/LGPD e Comitê/Auditoria):** Detalhada integralmente em [`reports/02_politica_ia_responsavel_taranis_black.md`](02_politica_ia_responsavel_taranis_black.md).
4. **Rota 3 — Etapa 1 Obrigatória (3 Personas, System Prompt Completo, Sessão SBI com 1ª e 2ª Tentativas e Avaliação de Eficácia):** Detalhada integralmente em [`simulator/prompt_simulador_sbi.md`](../simulator/prompt_simulador_sbi.md) e [`simulator/README.md`](../simulator/README.md).

---

## 6. Recomendação Futura de Expansão Interdepartamental (Roadmap Pós-MVP)

Como evolução estratégica após este MVP de RH, recomenda-se à CEO integrar os diagnósticos das **4 Rotas da Taranis Black**: atacar simultaneamente a automação de propostas e CRM no Comercial (Rota 1), a padronização de conteúdo no Marketing (Rota 2) e o redesenho Lean SIPOC/conciliação financeira em Operações e Finanças (Rota 4). Reduzir o atrito dos sistemas legados diminuirá o esgotamento estrutural das lideranças e potencializará os efeitos do treinamento SBI e do Onboarding Inteligente sobre a retenção e o eNPS.

---

## 7. Registro STAR de Portfólio (Metodologia hub-os-guIA)

* **Situação (S):** A Taranis Black (R$ 48M, 280 colaboradores) enfrentava turnover de 22,8% (23,4% a 24% nos primeiros 90 dias), queda de eNPS (+62 para +28) e dificuldades de líderes recém-promovidos em conduzir feedbacks difíceis sob forte sobrecarga operacional de sistemas legados.
* **Tarefa (T):** Estruturar em curto prazo a fundação estratégica de IA Responsável (Rota Zero) e implementar um MVP prático de Simulador de Liderança baseado no modelo SBI combinado com diagnóstico auditável de People Analytics (Rota 3).
* **Ação (A):** Execução de pipeline Bronze → Prata → Ouro em Python/Colab com anonimização na origem; mapeamento de 3 casos de uso no AI Canvas; priorização via Matriz Esforço × Impacto; redação de Política de IA Responsável alinhada à LGPD com Comitê de Auditoria; e engenharia de System Prompt com 3 personas desafiadoras, rubrica SBI de 0 a 10 e teste completo de 1ª e 2ª tentativas.
* **Resultado (R):** MVP executivo 100% documentado, auditado e demonstrável (com salto de 2,0 para 10,0 na sessão de teste da rubrica SBI e 3 gráficos executivos gerados); **impacto em redução de turnover real registrado como métrica futura a ser medida após implantação do piloto**, preservando rigor científico e transparência executiva.
