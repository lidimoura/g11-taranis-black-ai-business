# Catálogo de Prompts por Etapa & Guia Multi-LLM de Governança SBI — Challenge G11

![Status](https://img.shields.io/badge/Status-Validated_%26_Audited-success)
![Governance](https://img.shields.io/badge/Governance-Hub_OS_NEXUS_%7C_LGPD-blueviolet)
![Route](https://img.shields.io/badge/Route-Rota_Zero_%2B_Rota_3_(RH)-blue)

**Projeto:** G11 — Taranis Black | AI for Business (Oracle Next Education & Alura)  
**Responsável & Arquiteta de Soluções:** Lídi Moura (CEO, Encontro d'Água Hub)  
**Data:** 08–09/11/2026  

---

## 1. Diferença entre os Comandos Orquestradores (`ANTIGRAVITY_COMMAND`) e os Prompts por Etapa

Para total transparência documental e reprodutibilidade do projeto, este repositório preserva tanto os **Meta-Prompts Orquestradores** (usados para comandar o agente executor em fases) quanto os **Prompts Específicos de Cada Etapa** exigidos pela metodologia do Challenge G11:

| Arquivo no Repositório | Natureza do Artefato | Papel no Projeto |
| :--- | :--- | :--- |
| [`ANTIGRAVITY_COMMAND_MVP_G11.md`](../ANTIGRAVITY_COMMAND_MVP_G11.md) | **Meta-Prompt Orquestrador Inicial (v1.0)** | Especificação inicial preparada em conjunto com o Manus AI definindo o escopo enxuto do MVP, os entregáveis de código/documentação e as travas de segurança. Mantido na raiz para integridade histórica dos links. |
| [`ANTIGRAVITY_COMMAND_FINAL_G11.md`](../ANTIGRAVITY_COMMAND_FINAL_G11.md) | **Meta-Prompt Orquestrador Final por Fases (v2.0)** | Protocolo rigoroso de execução em **8 Fases (Fase 0 a Fase 7)** com checkpoints obrigatórios de aprovação da CEO Lídi Moura, mapeando cada linha do Template Oficial da Rota 3. |
| **`docs/CATALOGO_PROMPTS_POR_ETAPA_G11.md`** *(Este documento)* | **Catálogo Auditável de Prompts por Etapa** | Consolida os prompts modulares aplicados em cada etapa da **Rota Zero (Etapas 1, 2 e 3)** e da **Rota 3 (Etapas 1 e 2)**, além do protocolo de implantação segura do Simulador SBI em múltiplas LLMs. |
| [`simulator/prompt_simulador_sbi.md`](../simulator/prompt_simulador_sbi.md) | **System Prompt Oficial do Produto (Rota 3 — Etapa 1)** | O prompt de sistema completo do **Simulador de Liderança no Modelo SBI** com as 3 personas sintéticas, rubrica de 0 a 10 e *guardrails* LGPD. |

---

## 2. Registro Auditável de Prompts por Etapa (Rota Zero + Rota 3)

### 2.1. Etapa Diagnóstica & Rota 3 (Etapa 2) — People Analytics & Hipóteses Sem Causalidade
* **Ferramentas:** Python (`pandas`, `matplotlib`, `seaborn`) no Google Colab + Antigravity IDE.
* **Revisão Humana (HITL):** Conferência cruzada entre as 3 abas da planilha sintética (`Base_Colaboradores`, `Pesquisa_Clima_Qualitativa` e `KPIs_Gerais_RH`), remoção de `Nome` e `Salário Mensal (R$)` na Camada Prata e reconciliação da divergência entre `22,8%`, `23,4%` e `~24%`.
* **Prompt / Instrução Estruturada Aplicada:**
```markdown
Atue como Especialista Sênior em People Analytics e Governança de Dados (LGPD).
Sobre a base sintética da Taranis Black (280 colaboradores), execute uma arquitetura conceitual Bronze → Prata → Ouro:
1. Na Camada Prata, remova imediatamente colunas identificáveis ou sensíveis ('Nome' e 'Salário Mensal (R$)') antes de qualquer agregação.
2. Na Camada Ouro, calcule de forma determinística: turnover observado por departamento, desligamentos em até 90 dias, nota média de eNPS, absenteísmo médio anual, distribuição das causas reportadas nas entrevistas de saída (n=64) e médias das 3 dimensões da pesquisa qualitativa de clima (n=14).
3. Reconcilie com transparência metodológica eventuais diferenças entre o texto do enunciado (~24% turnover <90d), a aba consolidada de KPIs (23,4%) e a contagem estrita da base detalhada (13 casos <= 90 dias).
4. Formule 3 hipóteses diagnósticas conectando os achados de RH aos gargalos operacionais de sistemas legados da empresa (ERP lento, planilhas manuais e falta de rastreio de frete), sem jamais afirmar causalidade direta sem experimento controlado.
```

---

### 2.2. Rota Zero (Etapa 1) — AI Canvas, Tipos de IA e Supervisão Humana
* **Ferramentas:** Antigravity IDE + Manus AI + Governança Hub OS NEXUS.
* **Revisão Humana (HITL):** Validação pela CEO Lídi Moura garantindo visão sistêmica interdepartamental (reconhecendo que a própria liderança intermediária está sobrecarregada pelos sistemas legados).
* **Prompt / Instrução Estruturada Aplicada:**
```markdown
Atue como Consultora Executiva de IA para Negócios contratada pela CEO da Taranis Black (R$ 48M faturamento, 280 colaboradores, crescimento de 35% a.a.).
Com base no diagnóstico auditado de People Analytics, estruture a Etapa 1 da Rota Zero:
1. Construa o AI Canvas completo (Problema, Usuários, Dados com Privacy by Design, Solução, Proposta de Valor, Riscos e Controles) para 3 casos de uso complementares:
   - Caso 1 (Prioritário - Rota 3): Simulador de Liderança em Feedbacks Difíceis (Modelo SBI);
   - Caso 2 (Curto Prazo): Análise Assistida de Clima e Voz do Colaborador;
   - Caso 3 (Médio Prazo): Onboarding Inteligente 30-60-90 Dias (Assistente RAG).
2. Classifique tecnicamente cada iniciativa entre IA Generativa, IA Tradicional/Estatística e IA Preditiva (ou abordagem híbrida), justificando por que cálculos exatos devem ficar em código determinístico e interações semânticas em LLMs.
3. Defina os pontos inegociáveis de Supervisão Humana (Human-in-the-Loop) em conformidade com o Art. 20 da LGPD.
```

---

### 2.3. Rota Zero (Etapa 2) — Matriz Esforço × Impacto, Métricas de Sucesso e Gestão de Mudança
* **Ferramentas:** Antigravity IDE + Python (`matplotlib` para geração visual da Matriz 2×2).
* **Revisão Humana (HITL):** Calibração das metas para não prometer redução mágica de turnover e inclusão do cuidado com o esgotamento das lideranças na gestão de mudança.
* **Prompt / Instrução Estruturada Aplicada:**
```markdown
Estruture a Etapa 2 da Rota Zero para a Taranis Black:
1. Posicione os 3 casos de uso na Matriz Esforço × Impacto (2x2), justificando com dados reais da base por que o Simulador SBI é o Quick Win Estratégico nº 1 (ataca 40,6% das causas de saída sem depender de integração com o ERP legado).
2. Elabore o quadro de Métricas de Sucesso separando: Adoção (% de líderes treinados), Aprendizagem/Eficácia (evolução na rubrica SBI entre 1ª e 2ª tentativa), Horas Economizadas pelo RH/Gestores, Viabilidade/ROI estimado (custo evitado de reposição) e KPIs acompanhados no médio prazo.
3. Desenhe um Plano de Gestão de Mudança em 4 fases que proteja a segurança psicológica dos gestores (posicionando o simulador como 'Academia Segura de Liderança' e não como auditoria punitiva) e utilize formatos enxutos de microlearning (20 min) compatíveis com líderes já sobrecarregados.
```

---

### 2.4. Rota Zero (Etapa 3) — Política de IA Responsável, Riscos/LGPD e Comitê de Auditoria
* **Ferramentas:** Antigravity IDE + Diretrizes de Segurança Hub OS NEXUS.
* **Revisão Humana (HITL):** Verificação de aderência aos artigos 6º, 12, 20 e 46 da Lei nº 13.709/2018 (LGPD).
* **Prompt / Instrução Estruturada Aplicada:**
```markdown
Redija a Política Corporativa de IA Responsável da Taranis Black (Rota Zero — Etapa 3):
1. Estruture uma tabela prática e direta 'O QUE PODE vs. O QUE NÃO PODE' cobrindo o uso de ChatGPT, Gemini, Claude, Antigravity e Colab em RH, Comercial, Marketing e Operações (Tolerância Zero para envio de PII, salários, CPFs, segredos ou arquivos .env, e vedação absoluta a decisões automatizadas de RH).
2. Mapeie os riscos de Viés Algorítmico e Violações de LGPD (incluindo risco de reidentificação indireta em departamentos pequenos) e defina controles técnicos como remoção na Camada Prata e corte mínimo de k-anonymity (mínimo de 5 respondentes).
3. Defina a composição do Comitê Multidisciplinar de Governança de IA e Ética e estabeleça a cadência dos rituais de auditoria (Mensal para logs/prompts do piloto, Trimestral para LGPD/vieses e Semestral para revisão estratégica pela CEO).
```

---

### 2.5. Rota 3 (Etapa 1 Obrigatória) — Simulador de Feedbacks Difíceis no Modelo SBI
* **Prompt Completo Versionado:** Consulte integralmente [`simulator/prompt_simulador_sbi.md`](../simulator/prompt_simulador_sbi.md) e a sessão de teste em [`simulator/README.md`](../simulator/README.md).

---

## 3. Guia de Criação, Estruturação e Manutenção do Simulador SBI em Outras LLMs (Compliance & Governança)

O System Prompt do **Simulador de Liderança SBI** foi projetado de forma **agnóstica e portátil**. Abaixo estão as especificações práticas para implantar, manter e escalar o agente nas principais plataformas de LLMs do mercado mantendo 100% de conformidade com a Política de IA Responsável da Taranis Black:

| Plataforma / Ambiente | Como Criar e Estruturar (Passo a Passo) | Requisitos de Compliance, Segurança e Manutenção Contínua |
| :--- | :--- | :--- |
| **1. Google Gemini (Gems Corporativo)** | 1. Acessar o *Gem Manager* no Google Workspace.<br>2. Nomear como `Simulador SBI — Academia de Liderança Taranis Black`.<br>3. Colar o conteúdo de `simulator/prompt_simulador_sbi.md` nas Instruções.<br>4. Anexar `reports/02_politica_ia_responsavel_taranis_black.md` na base de conhecimento do Gem. | • **Vantagem de Compliance:** Dentro do Google Workspace Enterprise, as interações não são usadas para treinar modelos públicos externos e herdam o controle de acesso (RBAC) do domínio da empresa.<br>• **Manutenção:** Revisão mensal pelo BP de RH atualizando cenários conforme novos achados da pesquisa de clima. |
| **2. OpenAI ChatGPT (Custom GPTs)** | 1. Abrir o *GPT Builder* (`Configure`).<br>2. Inserir o System Prompt no campo `Instructions`.<br>3. Configurar 3 *Conversation Starters* guiados: `[Treinar Persona 1: Lucas - Comercial B2B]`, `[Treinar Persona 2: Marina - Suporte <90d]` e `[Treinar Persona 3: Rafael - Logística]`.<br>4. Desativar `Web Browsing` e `Code Interpreter` (desnecessários para o roleplay puro). | • **Requisito Crítico LGPD:** Em *Additional Settings*, desmarcar obrigatoriamente a caixa **"Use conversation data in your GPT to improve our models"**.<br>• Publicar apenas como *"Only people with a link"* ou interno da organização (Planos Team/Enterprise). |
| **3. Anthropic Claude (Claude Projects & Artifacts)** | 1. Criar um *Project* privado chamado `Treinamento Liderança SBI`.<br>2. Inserir o System Prompt em *Project Instructions*.<br>3. Solicitar que a tabela da Rubrica SBI (Critérios 1 a 5) seja renderizada em um *Artifact* visual lateral a cada tentativa. | • **Governança:** Operar em conta corporativa/Team com opt-out de treinamento.<br>• Ideal para sessões facilitadas ao vivo entre BP de RH e gestor pela excelente calibração de tom e nuança psicológica do modelo. |
| **4. Notebook Google Colab (`02_simulador_sbi_demo_governanca.ipynb`)** | Notebook interativo estruturado em Python que implementa uma **Camada de Sanitização Anti-PII (Pré-Prompt)** antes de avaliar o feedback do gestor (podendo rodar em modo demonstrativo determinístico sem chave ou conectado via `google.colab.userdata` ao Gemini API). | • **Tolerância Zero a Hardcoding:** Jamais inserir chaves de API diretamente no código; usar exclusivamente o gerenciador de segredos nativo do Colab (`userdata.get('GEMINI_API_KEY')`).<br>• **Filtro Regex Local:** Bloqueia automaticamente o envio caso o texto do usuário contenha padrões de CPF, e-mail ou nomes reais da base. |
