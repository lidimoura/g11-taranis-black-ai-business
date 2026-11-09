# AI Canvas & Mapeamento de Oportunidades — Taranis Black (Rota Zero + Rota 3)

**Projeto:** Challenge ONE G11 — AI for Business  
**Empresa Simulada:** Taranis Black (Ergonomia Corporativa — Linhas *ErgoPro*, *SmartDesk* e *Silence*)  
**Responsável:** Lídi Moura (Consultora Executiva de IA para Negócios)  
**Data:** 08/11/2026  

---

## 1. Visão Sistêmica e Contexto Interdepartamental

A Taranis Black cresceu 35% ao ano nos últimos três anos (atingindo R$ 48 milhões de faturamento e 280 colaboradores), mas sua infraestrutura operacional permaneceu apoiada em processos manuais, múltiplas planilhas e um ERP legado.

O diagnóstico de People Analytics revela que a dor do RH não é isolada: **Suporte ao Cliente (38,5% de turnover; eNPS +08)** e **Comercial B2B (30,9% de turnover; eNPS +18)** sofrem o impacto direto de gargalos sistêmicos documentados em todo o ecossistema da empresa (atrasos de até 48h na geração de propostas comerciais, perda de mais de 40% do tempo em preenchimento manual de CRM/planilhas, 5 dias de atraso no fechamento financeiro mensal e R$ 960 mil em fretes emergenciais sem visibilidade de rastreio para o atendimento).

> **Insight Estratégico da Consultoria (Visão Sistêmica):** As próprias lideranças intermediárias encontram-se sobrecarregadas por processos legados e cobranças operacionais, acabando por repassar essa pressão de forma reativa às equipes de linha de frente que lidam diretamente com a frustração do cliente externo. Portanto, a adoção de IA em RH deve **capacitar a liderança para absorver e conduzir tensões com empatia e método (Modelo SBI)**, ao mesmo tempo em que **sistematiza os sinais de esgotamento operacional** para evolução conjunta com Operações, Finanças e Comercial.

---

## 2. AI Canvas Corporativo — Os 3 Casos de Uso Mapeados

| Bloco do AI Canvas | Caso de Uso 1 (PRIORITÁRIO — Missão Rota 3)<br>**Simulador de Liderança em Feedbacks Difíceis (Modelo SBI)** | Caso de Uso 2 (COMPLEMENTAR — Diagnóstico)<br>**Análise Assistida de Clima e Voz do Colaborador** | Caso de Uso 3 (COMPLEMENTAR — Estruturação)<br>**Onboarding Inteligente 30-60-90 Dias (Assistente RAG)** |
| :--- | :--- | :--- | :--- |
| **1. Problema de Negócio** | Líderes recém-promovidos carecem de preparo prático para conversas difíceis; 40,6% dos desligamentos apontam falta de clareza nas metas e comunicação difícil com a liderança direta (nota 2,33/5 em Comercial B2B e Suporte). | Comentários abertos de clima e entrevistas de saída demoram a ser consolidados manualmente pelo RH, atrasando a detecção de esgotamento operacional (nota 2,07/5 em Carga de Trabalho e 2,43/5 em Ferramentas). | Turnover nos primeiros 90 dias chegou a 23,4% nos KPIs (~24% no enunciado), concentrado em Comercial B2B (29,4%) e Suporte (32,0%), com relatos de integração insuficiente e falta de playbooks iniciais. |
| **2. Usuários & Beneficiários** | **Diretos:** Gestores de equipe (especialmente líderes recém-promovidos de Comercial B2B, Suporte e Operações) e BPs de RH.<br>**Indiretos:** Colaboradores das equipes lideradas. | **Diretos:** Equipe de People Analytics, BPs de RH e Comitê Executivo.<br>**Indiretos:** Todos os 280 colaboradores e lideranças de área. | **Diretos:** Novos colaboradores (0 a 90 dias), líderes diretos ("padrinhos") e time de Gente & Cultura. |
| **3. Dados Necessários (Privacy by Design)** | • Cenários fictícios calibrados com dores reais agregadas da Taranis Black;<br>• Rubrica metodológica SBI (Situação, Comportamento, Impacto);<br>• **Zero dados pessoais (PII)** de colaboradores reais. | • Base quantitativa agregada (`Base_Colaboradores` sem Nome/Salário);<br>• Comentários qualitativos previamente **anonimizados e sanitizados**;<br>• Taxonomia de causas (Liderança, Processos/ERP, Carga, Remuneração). | • Catálogo técnico NR-17 (*ErgoPro, SmartDesk, Silence*);<br>• Playbooks operacionais, políticas internas e trilhas de 30-60-90 dias validados pelo RH;<br>• Dúvidas frequentes anonimizadas. |
| **4. Solução e Funcionamento** | Agente conversacional instruído por System Prompt estruturado que interpreta 3+ personas desafiadoras em *roleplay*, avalia o feedback do gestor segundo 5 critérios da rubrica SBI, oferece coaching construtivo e exige uma 2ª tentativa prática. | Pipeline analítico (Python/Colab + LLM sob supervisão) que cruza indicadores departamentais com clusterização temática e análise de sentimento agregada dos relatos abertos, gerando planos de ação por diretoria. | Assistente virtual baseado em RAG (*Retrieval-Augmented Generation*) restrito a documentos oficiais da Taranis Black para responder dúvidas de processo/produto no fluxo de trabalho e guiar marcos de 30, 60 e 90 dias. |
| **5. Proposta de Valor & Impacto Esperado** | • Ambiente psicologicamente seguro ("academia de liderança") para errar e ajustar o tom antes da conversa real;<br>• Padronização da cultura de feedback objetivo (foco no comportamento, não no rótulo pessoal);<br>• Redução de ruídos e conflitos em equipes sob alta pressão. | • Redução de ~70% no tempo manual do RH para categorizar pesquisas qualitativas;<br>• Visibilidade executiva imediata sobre como gargalos de ERP/logística afetam a retenção;<br>• Insumo contínuo para atualizar cenários do Simulador SBI. | • Aceleração da curva de ramp-up em Comercial B2B e Suporte;<br>• Redução da sensação de desamparo nos regimes Híbrido (26,6% turnover) e Remoto (26,5%);<br>• Alívio da carga repetitiva de treinamento sobre líderes esgotados. |
| **6. Riscos Mapeados** | • Uso indevido do simulador como ferramenta punitiva ou de avaliação formal de gestores;<br>• Inserção acidental de nomes/casos reais identificáveis pelo gestor;<br>• Respostas estereotipadas da IA ou tentativa de usar o agente para casos graves (assédio/saúde mental). | • Risco de reidentificação indireta em departamentos pequenos (ex.: Gente e Cultura com 15 pessoas);<br>• Alucinação interpretativa ou viés de confirmação;<br>• Percepção de vigilância se os comentários não forem agregados. | • Desatualização da base documental gerando orientações operacionais incorretas;<br>• Substituição indevida do acolhimento humano do gestor pelo chatbot;<br>• Coleta excessiva de logs individuais de dúvidas dos novatos. |
| **7. Controles & Governança (LGPD / HITL)** | • Trava explícita no System Prompt proibindo decisões de RH;<br>• Uso exclusivo de personas sintéticas;<br>• Gatilho automático de escalonamento ao BP de RH em temas sensíveis;<br>• Curadoria humana periódica da rubrica. | • Corte mínimo de agregação (`k-anonymity`: mínimo de 5 respondentes para exibir recortes qualitativos);<br>• Remoção de PII na Camada Prata;<br>• Revisão obrigatória por Analista de People Analytics antes de envio à CEO. | • Arquitetura RAG restrita a documentos aprovados (sem treino externo);<br>• Rituais humanos obrigatórios de 1:1 aos 15, 30, 60 e 90 dias;<br>• Logs de dúvidas armazenados apenas de forma estatística agregada. |

---

## 3. Classificação por Tipo de IA e Justificativa Técnica

| Iniciativa / Caso de Uso | Classificação Principal de IA | Componentes Combinados | Justificativa Técnica da Escolha |
| :--- | :--- | :--- | :--- |
| **1. Simulador de Feedbacks Difíceis (Modelo SBI)** | **IA Generativa** (*LLMs Conversacionais*) | Engenharia de System Prompt Avançada + Rubrica Determinística de Avaliação (Critérios 1 a 5) | O treinamento de conversas difíceis exige interpretação de nuances de linguagem natural, adaptação dinâmica ao tom do gestor (*roleplay* realista) e geração de feedback pedagógico personalizado — tarefas exclusivas da **IA Generativa**, ancoradas por uma rubrica estruturada para evitar subjetividade. |
| **2. Análise Assistida de Clima e Diagnóstico de People Analytics** | **Híbrida: IA Tradicional (Estatística/Regras) + IA Generativa (NLP)** *(com evolução futura para IA Preditiva)* | • **IA Tradicional / Ciência de Dados:** Agregações determinísticas em Python/Colab (taxas de turnover, médias, cruzamentos);<br>• **IA Generativa (NLP):** Sumarização temática e sentimento em textos abertos;<br>• **IA Preditiva (Roadmap futuro):** Modelos de propensão a *attrition* por coorte agregada. | Cálculos de KPIs de RH exigem exatidão matemática auditável (**IA Tradicional/Estatística**, onde LLMs não devem calcular sozinhos para evitar alucinação numérica), enquanto a leitura de comentários abertos se beneficia da capacidade semântica da **IA Generativa**. Modelos de **IA Preditiva** ficam no roadmap apenas para estimar risco agregado de área, nunca para rotular indivíduos. |
| **3. Onboarding Inteligente (Primeiros 90 Dias)** | **IA Generativa com RAG** + **IA Tradicional (Fluxos Baseados em Regras)** | • **RAG (*Retrieval-Augmented Generation*):** Busca semântica sobre manuais NR-17 e playbooks;<br>• **Automação Tradicional:** Disparo programado de checklists de 30/60/90 dias. | O novato precisa de respostas precisas e fiéis aos manuais da Taranis Black (**IA Generativa com RAG** para mitigar alucinações), combinadas com gatilhos temporais simples e previsíveis (**IA Tradicional baseada em regras**) para lembretes de integração. |

---

## 4. Supervisão Humana Obrigatória (*Human-in-the-Loop* — HITL)

Em conformidade com o **Art. 20 da LGPD** e com as diretrizes de ética corporativa da Taranis Black, **nenhuma iniciativa de IA em RH opera em modo 100% autônomo sobre decisões relativas a pessoas**:

1. **No Simulador SBI (Caso 1):**
   - **Papel do Humano:** BPs de RH desenham e auditam as personas e a rubrica; facilitadores humanos conduzem rodas de debriefing com os líderes após as simulações; casos reais envolvendo suspeita de assédio moral/sexual, discriminação, sofrimento psíquico/burnout agudo ou medidas disciplinares possuem **bloqueio de simulação** e exigem condução direta e presencial do RH e Jurídico.
2. **Na Análise Assistida de Clima (Caso 2):**
   - **Papel do Humano:** A IA atua apenas como copiloto de triagem e síntese estatística/temática. O Analista de People Analytics confere a integridade dos cálculos no notebook Colab, valida se nenhum trecho qualitativo permite reidentificação indireta e interpreta o contexto organizacional antes de submeter recomendações à CEO.
3. **No Onboarding Inteligente (Caso 3):**
   - **Papel do Humano:** Gente & Cultura aprova e versiona os documentos da base de conhecimento; o assistente virtual responde dúvidas operacionais, mas os check-ins de adaptação cultural e definição de metas aos 30, 60 e 90 dias são realizados obrigatoriamente pelo líder humano e pelo BP da área.
