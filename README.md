# 🌿 G11 — Taranis Black | AI for Business (Rota Zero + Rota 3: RH & People Analytics)

![Status](https://img.shields.io/badge/Status-MVP_Delivered_%26_Audited-success)
![Program](https://img.shields.io/badge/Program-Oracle_Next_Education_(ONE)_G11_%7C_Alura-orange)
![Tech Stack](https://img.shields.io/badge/Tech_Stack-Python_%7C_Pandas_%7C_Colab_%7C_Prompt_Engineering-blue)
![Governance](https://img.shields.io/badge/Governance-Hub_OS_NEXUS_%7C_LGPD_%7C_Human--in--the--Loop-blueviolet)
![Languages](https://img.shields.io/badge/Docs-PT--BR_%7C_EN_%7C_ES-teal)
![License](https://img.shields.io/badge/Scope-Educational_Synthetic_Data-lightgrey)

> 🌐 **Select Language / Seleccione el Idioma / Selecione o Idioma:**  
> [🇧🇷 Português](#-visão-geral-do-projeto-pt-br) | [🇺🇸 English](#-project-overview-en) | [🇪🇸 Español](#-descripción-general-del-proyecto-es)

---

> **Nota de Transparência & Governança:** Este projeto foi idealizado, direcionado e auditado por **Lídi Moura** (CEO, PO e Arquiteta de Soluções do **Encontro d'Água Hub**), integrando execução analítica no **Google Colab/Python**, execução técnica e QA no **Antigravity IDE**, preparação inicial no **Manus AI** e as camadas autorais de governança **Hub OS NEXUS** e **hub-os-guIA**. Todos os dados da empresa simulada **Taranis Black** são 100% sintéticos para fins educacionais, tratados sob rigorosa anonimização (*Privacy by Design* / LGPD).

---

## 🇧🇷 Visão Geral do Projeto (PT-BR)

A **Taranis Black** é uma empresa brasileira simulada de ergonomia corporativa (linhas *ErgoPro*, *SmartDesk* e *Silence*), com faturamento anual de **R$ 48 milhões**, **280 colaboradores** e crescimento acelerado de **35% ao ano**. Esse crescimento apoiado em processos manuais legados gerou desgaste severo:
* **Turnover anual geral:** `22,8%` na aba de KPIs (`22,9%` / 64 desligamentos na base detalhada);
* **Turnover nos primeiros 90 dias:** `23,4%` nos KPIs consolidados (`~24%` reportado no enunciado e `13 casos ≤ 90d` na filtragem estrita da base);
* **Queda do eNPS corporativo:** de `+62` para `+28` (chegando a `+08` em Suporte ao Cliente e `+18` em Comercial B2B);
* **Causas nº 1 e nº 2 nas entrevistas de saída (`n = 64`):** *Falta de clareza nas metas e comunicação difícil com a liderança direta* (**40,6%**) e *Sobrecarga com tarefas manuais e sistemas lentos* (**31,2% geral**, subindo para **46,2%** nos desligados em até 90 dias).

### 🧠 Visão Sistêmica da Consultoria
Nossa análise demonstra que **as próprias lideranças intermediárias estão esgotadas pelos processos legados da Taranis Black** (ERP demorando 48h para gerar propostas comerciais, perda de 40% do tempo comercial em planilhas, 5 dias de atraso no fechamento financeiro e falta de rastreamento de fretes emergenciais) e acabam transferindo essa pressão para as equipes de linha de frente (**Suporte ao Cliente: 38,5% de turnover** e **Comercial B2B: 30,9%**).

---

### 🎯 Arquitetura da Solução (Rota Zero + Rota 3)

| Camada / Iniciativa | Classificação de IA | Prioridade (Matriz Esforço × Impacto) | Entregável / Evidência no Repositório |
| :--- | :--- | :--- | :--- |
| **1. Simulador de Liderança em Feedbacks Difíceis (Modelo SBI)** | **IA Generativa** (LLM Conversacional) + Rubrica Determinística (0 a 10) | **1º Lugar — Quick Win Estratégico** *(Alto Impacto / Médio Esforço)* | [`simulator/prompt_simulador_sbi.md`](simulator/prompt_simulador_sbi.md)<br>[`simulator/README.md`](simulator/README.md)<br>[`notebooks/02_simulador_sbi_demo_governanca.ipynb`](notebooks/02_simulador_sbi_demo_governanca.ipynb) |
| **2. Análise Assistida de Clima e Diagnóstico People Analytics** | **Híbrida:** IA Tradicional/Estatística (Colab) + IA Generativa (NLP) | **2º Lugar — Alavanca Diagnóstica** *(Médio-Alto Impacto / Baixo-Médio Esforço)* | [`notebooks/01_people_analytics_mvp.ipynb`](notebooks/01_people_analytics_mvp.ipynb)<br>[`outputs/`](outputs/README.md) |
| **3. Onboarding Inteligente 30-60-90 Dias** | **IA Generativa com RAG** + Automação Tradicional por Regras | **3º Lugar — Projeto Estruturante** *(Alto Impacto / Alto Esforço)* | [`docs/AI_CANVAS_R0_R3.md`](docs/AI_CANVAS_R0_R3.md)<br>[`reports/03_plano_metricas_e_gestao_mudanca.md`](reports/03_plano_metricas_e_gestao_mudanca.md) |
| **Fundação Ética, Política "Pode / Não Pode" & Comitê LGPD** | Governança Corporativa, *k-anonymity* e *Human-in-the-Loop* (Art. 20 LGPD) | **Base Obrigatória Inegociável (Rota Zero)** | [`reports/02_politica_ia_responsavel_taranis_black.md`](reports/02_politica_ia_responsavel_taranis_black.md)<br>[`docs/CATALOGO_PROMPTS_POR_ETAPA_G11.md`](docs/CATALOGO_PROMPTS_POR_ETAPA_G11.md) |

---

### 🚀 Features de Evolução & Roadmap Pós-Entrega (Próximos Passos Planejados)

Mantendo total transparência sobre o que compõe a entrega validada do MVP hoje e as expansões arquitetadas para o ciclo pós-challenge:

- [x] **MVP Entregue (Rota 0 + Rota 3):** Diagnóstico auditável Bronze→Prata→Ouro em Python, AI Canvas, Matriz Esforço × Impacto, Política de IA Responsável (LGPD), Simulador SBI com 3 personas sintéticas (*Lucas Andrade, Marina Costa e Rafael Mendes*), sessão completa de 1ª e 2ª tentativas (`2,0/10 → 10,0/10`) e Showcase HTML.
- [ ] **Feature Futura 1 — Criação Guiada, Estruturação e Manutenção Multi-LLM do Simulador SBI:** Expansão do agente SBI para operação assistida em **Google Gemini Gems** (Workspace corporativo), **OpenAI Custom GPTs** e **Claude Projects/Artifacts**, acompanhada do notebook [`notebooks/02_simulador_sbi_demo_governanca.ipynb`](notebooks/02_simulador_sbi_demo_governanca.ipynb) com filtro pré-prompt Anti-PII em Python e gestão segura de chaves via `colab.userdata` (veja especificação completa em [`docs/CATALOGO_PROMPTS_POR_ETAPA_G11.md`](docs/CATALOGO_PROMPTS_POR_ETAPA_G11.md)).
- [ ] **Feature Futura 2 — Diagnóstico Holístico Integrado (Rotas 1, 2, 3 e 4 da Taranis Black):** Cruzamento dos indicadores de People Analytics (Rota 3) com o Playbook de Objeções Comerciais B2B (Rota 1), o Guia de Tom de Voz de Marketing (Rota 2) e o mapeamento Lean SIPOC / Diagrama de Ishikawa do fechamento financeiro e fretes (Rota 4), atacando simultaneamente o preparo humano da liderança e a modernização dos sistemas legados que geram sobrecarga.

---

### 🗂️ Estrutura Organizacional do Repositório

```text
g11-taranis-black-ai-business/
├── docs/
│   ├── AI_CANVAS_R0_R3.md                     # AI Canvas, Tipos de IA e Supervisão Humana (HITL)
│   ├── CATALOGO_PROMPTS_POR_ETAPA_G11.md      # Prompts de cada etapa + Guia Multi-LLM de Governança SBI
│   └── MVP_ARCHITECTURE.md                    # Arquitetura conceitual Bronze → Prata → Ouro
├── notebooks/
│   ├── 01_people_analytics_mvp.ipynb          # Análise principal de People Analytics (executada e sem PII)
│   └── 02_simulador_sbi_demo_governanca.ipynb # Demo do Simulador SBI + Filtro Anti-PII em Python e Colab Secrets
├── outputs/
│   ├── 01_turnover_por_departamento.png       # Gráfico: Turnover observado por departamento
│   ├── 02_clima_dimensoes_agregadas.png       # Gráfico: Médias da pesquisa qualitativa de clima (1 a 5)
│   ├── 03_motivos_desligamento_agregados.png  # Gráfico: Causas reportadas nas entrevistas de saída (n=64)
│   ├── 04_matriz_esforco_impacto.png          # Gráfico: Matriz 2x2 Esforço × Impacto (Rota Zero)
│   └── README.md                              # Documentação e governança LGPD dos visuais
├── reports/
│   ├── 01_relatorio_executivo_g11.md          # Relatório Executivo Integrado para a CEO + Registro STAR
│   ├── 02_politica_ia_responsavel_taranis_black.md # Política Pode/Não Pode, Riscos LGPD e Comitê de Auditoria
│   └── 03_plano_metricas_e_gestao_mudanca.md  # Matriz, ROI/Horas economizadas e Plano de Mudança em 4 fases
├── simulator/
│   ├── prompt_simulador_sbi.md                # System Prompt completo + 3 Personas Sintéticas
│   └── README.md                              # Sessão completa de teste SBI (1ª e 2ª tentativas) + Eficácia
├── showcase/
│   ├── index.html                             # Página visual executiva (Dark Mode / Glassmorphism)
│   └── README.md                              # Guia de visualização local do Showcase
├── ANTIGRAVITY_COMMAND_MVP_G11.md             # Meta-prompt orquestrador inicial (v1.0)
├── ANTIGRAVITY_COMMAND_FINAL_G11.md           # Meta-prompt orquestrador final em 8 fases (v2.0)
├── DELIVERY_QA_CHECKLIST_G11.md               # Checklist de QA e auditoria final (100% validado)
└── SOURCE_ACCESS_PROTOCOL_G11.md              # Protocolo de acesso seguro às fontes e contingência Drive
```

---

## 🇺🇸 Project Overview (EN)

**G11 — Taranis Black | AI for Business** is an executive AI consulting MVP developed for the **Oracle Next Education (ONE G11) & Alura Challenge** by **Lídi Moura** (CEO & Solutions Architect at **Encontro d'Água Hub**).

### Business Problem & Systemic Insight
**Taranis Black** is a simulated Brazilian corporate ergonomics company (BRL 48M annual revenue, 280 employees, growing 35% YoY). Rapid growth on top of manual legacy processes led to a **22.8% annual turnover** (**23.4% to ~24% within the first 90 days**) and an **eNPS drop from +62 to +28**.  
Our Python/Colab People Analytics pipeline revealed that **Customer Support (38.5% turnover)** and **B2B Sales (30.9% turnover)** account for **65.6% of all exits**, driven by two interconnected root causes:
1. **Unclear goals and difficult communication with newly promoted leaders (40.6% of exits)**;
2. **Overload from manual tasks and slow legacy ERP/spreadsheets (31.2% overall; 46.2% among ≤90-day exits; 2.07/5 workload climate score)**.

> **Systemic Consulting Insight:** Middle managers themselves are exhausted by legacy operational bottlenecks (48h ERP quote delays, manual financial reconciliation, lack of freight tracking) and inadvertently pass that pressure onto frontline teams.

### Key Deliverables (Route Zero + Route 3: HR & People Analytics)
1. **SBI Leadership Feedback Simulator (Priority 1 — Route 3):** A dual-mode conversational agent (Roleplay Actor + Pedagogical HR Mentor) featuring **3 synthetic personas** (*Lucas Andrade — B2B Sales*, *Marina Costa — Customer Support <90d*, and *Rafael Mendes — Operations/Logistics*), a **0–10 deterministic SBI Rubric** (*Situation, Behavior, Impact, Active Listening, Next Step*), mandatory second-attempt coaching loop, and strict LGPD/Human-in-the-Loop guardrails.
2. **Auditable People Analytics Pipeline (`Bronze → Silver → Gold`):** Reproducible Google Colab notebook that programmatically strips PII (`Name`, `Monthly Salary`) in the Silver layer and reconciles dataset metrics transparently.
3. **Responsible AI Policy, Effort × Impact Matrix & Change Management (Route Zero):** Practical *"Do's and Don'ts"* policy compliant with Brazil's **LGPD (Articles 6, 12, 20, and 46)**, multidisciplinary AI Ethics Committee, and a 4-phase change management plan focused on psychological safety.
4. **Post-MVP Roadmap:** Guided multi-LLM deployment of the SBI Simulator across **Google Gemini Gems, OpenAI Custom GPTs, Claude Projects, and Colab Secrets** ([`docs/CATALOGO_PROMPTS_POR_ETAPA_G11.md`](docs/CATALOGO_PROMPTS_POR_ETAPA_G11.md)), followed by cross-departmental integration with Sales, Marketing, and Lean Operations/Finance routes.

---

## 🇪🇸 Descripción General del Proyecto (ES)

**G11 — Taranis Black | AI for Business** es un MVP ejecutivo de consultoría en Inteligencia Artificial desarrollado para el **Challenge Oracle Next Education (ONE G11) & Alura** por **Lídi Moura** (CEO y Arquitecta de Soluciones en **Encontro d'Água Hub**).

### Problema de Negocio y Visión Sistémica
**Taranis Black** es una empresa brasileña simulada de ergonomía corporativa (facturación anual de R$ 48 millones, 280 colaboradores y crescimento del 35% anual). El crecimiento acelerado sobre procesos manuales heredados generó una **rotación (turnover) anual del 22,8%** (**23,4% a ~24% en los primeros 90 días**) y una caída del **eNPS de +62 a +28**.  
Nuestro diagnóstico en Python/Colab demostró que **Soporte al Cliente (38,5% de rotación)** y **Comercial B2B (30,9%)** concentran el **65,6% de las salidas**, impulsadas por:
1. **Falta de claridad en las metas y comunicación difícil con líderes recién promovidos (40,6% de las bajas)**;
2. **Sobrecarga por tareas manuales y lentitud del ERP heredado (31,2% general; 46,2% en bajas ≤90 días; nota de clima de 2,07/5 en Carga de Trabajo)**.

> **Visión Sistémica:** Los propios líderes intermedios están agotados por los cuellos de botella operativos (demoras de 48h en el ERP, planillas manuales y falta de rastreo logístico) y terminan trasladando esa presión a los equipos de atención y ventas.

### Entregables Principales (Ruta Cero + Ruta 3: RR.HH. y People Analytics)
1. **Simulador de Liderazgo en Feedbacks Difíciles — Modelo SBI (Prioridad 1):** Agente conversacional de doble rol (Actor de Roleplay + Mentor Pedagógico de RR.HH.) con **3 personas sintéticas**, rúbrica determinística SBI de 0 a 10 puntos, ciclo obligatorio de segundo intento y barreras éticas de privacidad y supervisión humana (*Human-in-the-Loop*).
2. **Pipeline Auditable de People Analytics (`Bronce → Plata → Oro`):** Notebook reproducible en Google Colab con anonimización programática en origen y gráficos ejecutivos de alta resolución.
3. **Política de IA Responsable, Matriz Esfuerzo × Impacto y Gestión del Cambio (Ruta Cero):** Directrices prácticas *"Qué se puede / Qué no se puede hacer"*, cumplimiento de la **LGPD**, Comité de Auditoría y plan de cambio en 4 fases.
4. **Hoja de Ruta Pos-MVP (Roadmap):** Implementación guiada del Simulador SBI en múltiples LLMs (**Gemini Gems, Custom GPTs, Claude Projects y Colab Secrets**) e integración futura con las demás áreas de negocio (Comercial, Marketing y Operaciones/Finanzas Lean).

---

## 🔗 Links Oficiais — Lídi Moura & Encontro d'Água Hub

| Canal / Ativo | Link Oficial |
| :--- | :--- |
| 📄 **Entrega Oficial Google Docs (Rota 0 + Rota 3)** | [Abrir Relatório Executivo no Google Docs](https://docs.google.com/document/d/1iJJCuZXFhak77p6Weirg4zp6UFpFhHxqaqFswUGZvAw/edit?usp=sharing) |
| 📓 **Notebook 01 — People Analytics (Google Colab)** | [Abrir no Google Colab](https://colab.research.google.com/github/lidimoura/g11-taranis-black-ai-business/blob/main/notebooks/01_people_analytics_mvp.ipynb) |
| 🤖 **Notebook 02 — Simulador SBI & Governança LGPD (Colab)** | [Abrir no Google Colab](https://colab.research.google.com/github/lidimoura/g11-taranis-black-ai-business/blob/main/notebooks/02_simulador_sbi_demo_governanca.ipynb) |
| 🌐 **Portfólio Hub & Serviços** | [https://link.encontrodagua.com/r/portifolio-lidimoura](https://link.encontrodagua.com/r/portifolio-lidimoura) |
| 💼 **LinkedIn Oficial** | [https://www.linkedin.com/in/lidimoura/](https://www.linkedin.com/in/lidimoura/) |
| 📲 **Link d'Água Pessoal (PT / EN)** | [PT-BR](https://link.encontrodagua.com/r/lidi-moura) \| [EN](https://link.encontrodagua.com/r/lidi-moura-en) |
| 🎨 **Behance** | [https://www.behance.net/lidimoura](https://www.behance.net/lidimoura) |
| 💻 **GitHub** | [https://github.com/lidimoura](https://github.com/lidimoura) |

---
*Encontro d'Água Hub OS — Reflorestando o Digital com Inteligência Artificial Responsável.*
