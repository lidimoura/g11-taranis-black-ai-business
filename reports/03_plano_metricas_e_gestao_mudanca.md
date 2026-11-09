# Plano de Priorização, Métricas de Sucesso e Gestão de Mudança — Taranis Black (Rota Zero — Etapa 2)

**Projeto:** Challenge ONE G11 — AI for Business  
**Empresa Simulada:** Taranis Black  
**Responsável:** Lídi Moura  
**Data:** 08/11/2026  

---

## 1. Matriz Esforço × Impacto e Ordem de Implantação

A priorização das iniciativas de IA na Taranis Black foi estruturada cruzando a gravidade dos achados quantitativos da base de People Analytics (`n = 280`) com a viabilidade técnica, o custo de implementação e a maturidade cultural atual da organização.

### 1.1. Matriz de Priorização (2×2)

| Ordem | Iniciativa de IA | Impacto no Negócio | Esforço de Implantação | Quadrante Estratégico | Justificativa Baseada em Dados |
| :---: | :--- | :---: | :---: | :--- | :--- |
| **1º** | **Simulador de Liderança em Feedbacks Difíceis (Modelo SBI)** | **Alto** | **Médio (Baixo Custo Técnico)** | **Quick Win Estratégico (Implantação Imediata — Semanas 1 a 4)** | Ataca diretamente a causa nº 1 reportada nas entrevistas de saída (**40,6% dos desligamentos**: *falta de clareza nas metas e comunicação difícil com a liderança*) e a nota crítica de liderança em Comercial B2B e Suporte (`2,33/5`). Não exige integração com o ERP legado, utiliza zero dados pessoais reais (opera 100% com personas sintéticas) e cumpre a missão obrigatória da Rota 3. |
| **2º** | **Análise Assistida de Clima e Voz do Colaborador** | **Médio / Alto** | **Baixo / Médio** | **Alavanca Diagnóstica Contínua (Semanas 3 a 8)** | Sistematiza rapidamente as dores de Carga de Trabalho (`2,07/5`) e Ferramentas/Processos (`2,43/5`), que respondem por **31,2% dos desligamentos gerais** e **46,2% das saídas em até 90 dias**. Aproveita o pipeline Python/Colab já construído no MVP e alimenta o Comitê Executivo com evidências interdepartamentais. |
| **3º** | **Onboarding Inteligente 30-60-90 Dias (Assistente RAG)** | **Alto** | **Alto** | **Projeto Estruturante de Médio Prazo (Meses 2 a 6)** | Tem alto potencial para reduzir a vulnerabilidade nos primeiros 90 dias (23,4% nos KPIs / ~24% no enunciado) e apoiar os regimes Híbrido (`26,6%` turnover) e Remoto (`26,5%`). Contudo, exige esforço prévio de higienização documental, estruturação de playbooks comercias/suporte e governança de acesso RAG, devendo entrar após a capacitação inicial das lideranças. |

---

## 2. Plano de Métricas de Sucesso, Metas de Adoção e Viabilidade (ROI Estimado)

> **Regra de Rigor Analítico:** Este MVP **não afirma que a implantação do simulador já reduziu o turnover**. Os indicadores abaixo estabelecem a linha de base (*baseline*) verificada nos dados atuais da Taranis Black e definem **como medir adoção, aprendizagem, eficiência operacional e impacto futuro no negócio** mediante experimentação controlada.

### 2.1. Quadro Geral de Métricas por Dimensão e Iniciativa

| Iniciativa | Métricas de Adoção e Engajamento | Métricas de Aprendizagem e Qualidade (Eficácia) | Horas Economizadas / Eficiência Operacional | Métricas de Negócio e Clima Monitoradas (Médio Prazo) | Estimativa de Viabilidade / Hipótese de ROI |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Simulador de Liderança SBI** *(Prioridade 1)* | • **Meta Piloto (30 dias):** ≥ 85% dos gestores de Suporte ao Cliente e Comercial B2B concluindo ao menos 3 cenários completos.<br>• **Meta Expansão (90 dias):** ≥ 80% de toda a liderança da Taranis Black treinada. | • **Evolução na Rubrica SBI (0 a 10):** Aumento médio de ≥ +2,5 pontos entre a 1ª tentativa e a 2ª tentativa na sessão simulada.<br>• **CSAT do Treinamento:** ≥ 4,2 / 5,0 de utilidade prática percebida pelos gestores. | • **~4h a 6h poupadas por BP de RH por ciclo** em roleplays individuais básicos, liberando o BP para mediação de casos complexos e mentoria avançada.<br>• Redução de retrabalho por feedbacks mal conduzidos. | • Evolução da **Nota de Liderança Direta** na pesquisa de clima (Baseline geral: `3,07/5`; Suporte/Comercial: `2,33/5` → Meta: `≥ 3,60/5` em 6 meses).<br>• Queda na proporção de saídas por *"comunicação difícil com liderança"* (Baseline: `40,6%`). | **Custo do Piloto:** Baixo (uso de licenças corporativas LLM já previstas + horas internas de RH).<br>**Hipótese de Retorno:** Cada desligamento evitado em cargos comerciais/técnicos preserva entre 1,5x e 3x o salário mensal em custos de reposição e rampa. Evitar apenas 3 a 5 saídas precoces no semestre já paga integralmente o programa. |
| **2. Análise Assistida de Clima** *(Prioridade 2)* | • **100% dos ciclos trimestrais** de pesquisa de clima e entrevistas de saída processados pelo pipeline padronizado Bronze → Prata → Ouro. | • **Taxa de Conformidade LGPD:** 100% dos relatórios sem exposição de PII.<br>• **Precisão Temática Validada pelo RH:** ≥ 90% de concordância na revisão humana amostral. | • **~12h a 16h economizadas por ciclo mensal/trimestral** de People Analytics na tabulação, limpeza e categorização qualitativa. | • Tempo entre fechamento da pesquisa de clima e entrega do plano de ação departamental reduzido de **15 dias para 3 dias úteis**. | **Alto retorno operacional imediato:** Transforma dados antes subutilizados em diagnósticos acionáveis para atacar gargalos de ERP/processos legados junto às demais diretorias. |
| **3. Onboarding Inteligente 90d** *(Prioridade 3)* | • **≥ 75% dos novos contratados** interagindo ativamente com a trilha de 30-60-90 dias nos dois primeiros meses. | • **Taxa de Resolução de Dúvidas Operacionais:** ≥ 80% das dúvidas sobre catálogo NR-17 e rotinas respondidas com base documental oficial. | • **~3h/semana poupadas por líder/padrinho** na repetição de instruções operacionais básicas durante o primeiro mês do novato. | • **Turnover nos Primeiros 90 Dias** (Baseline KPIs: `23,4%` geral; `32,0%` Suporte; `29,4%` Comercial → Meta estrutural: convergir para `< 15%` após 6 meses de operação integrada).<br>• Recuperação gradual do **eNPS** (Baseline: `+28` → Meta: `> +45`). | **Retorno estrutural de médio prazo:** Acelera a produtividade de novos SDRs e analistas de suporte, reduzindo perdas comerciais na ponta. |

---

## 3. Plano de Gestão de Mudança (Mitigação de Resistência Cultural e Esgotamento)

A análise integrada da Taranis Black mostra que **as próprias lideranças intermediárias estão pressionadas por metas altas e processos legados manuais**. Se o Simulador SBI ou as ferramentas de IA forem comunicados como "mais uma cobrança burocrática" ou como "auditoria para punir maus gestores", haverá forte resistência cultural. O plano de mudança abaixo atua em **4 fases práticas**:

### Fase 1 — Alinhamento Executivo e Segurança Psicológica (Semanas 1 e 2)
* **Mensagem-Chave da CEO e Gente & Cultura:** Posicionar oficialmente o Simulador SBI como uma **"Academia Segura de Liderança"** (*Flight Simulator*), e nunca como ferramenta de avaliação de desempenho, ranqueamento ou punição.
* **Reconhecimento da Sobrecarga Sistêmica:** Comunicar com transparência que a diretoria reconhece o desgaste causado pelos sistemas legados (ERP/planilhas) e que o programa de IA atua em duas frentes: apoiar o líder nas conversas difíceis do dia a dia e mapear os gargalos operacionais para alívio de carga.
* **Garantia de Privacidade:** Deixar claro que os treinos usam personas 100% fictícias e que os gestores não são julgados por errarem na 1ª tentativa da simulação (o erro faz parte do método pedagógico).

### Fase 2 — Piloto Controlado com "Líderes Champions" (Semanas 3 e 4)
* **Foco nas Áreas Críticas:** Iniciar com um grupo piloto de 8 a 12 coordenadores e supervisores de **Suporte ao Cliente** e **Comercial B2B**.
* **Formato Mão na Massa (Microlearning de 20 minutos):** Em vez de treinamentos teóricos longos que tomam a agenda do gestor, aplicar sessões curtas de 20 minutos onde o líder pratica 1 persona no simulador, recebe a rubrica SBI na hora e testa a 2ª tentativa.
* **Co-criação:** Ouvir os líderes do piloto para ajustar o vocabulário das personas à realidade do chão de fábrica/escritório da Taranis Black.

### Fase 3 — Capacitação Ampliada e Rituais de Troca (Mês 2)
* **Rodas Quinzenais de Prática Facilitadas por BPs:** Encontros breves entre pares para discutir aprendizados agregados (ex.: como substituir broncas coletivas em grupos de mensagens por feedbacks individuais estruturados em Situação-Comportamento-Impacto).
* **Integração com Clima:** Apresentar aos gestores os relatórios agregados da Análise Assistida de Clima como ferramenta de apoio à gestão deles, e não de fiscalização.

### Fase 4 — Consolidação, Governança Contínua e Evolução (Meses 3 a 6)
* **Incorporação ao Onboarding de Novos Líderes:** Todo colaborador promovido a cargo de gestão passa pela trilha prática do Simulador SBI antes de assumir a condução formal de ciclos de feedback.
* **Revisão pelo Comitê de IA:** Avaliação trimestral das métricas de adoção, evolução das notas SBI e escuta ativa das equipes para calibrar os próximos passos do roadmap (como o Onboarding Inteligente de 90 dias e as melhorias de processos interdepartamentais).
