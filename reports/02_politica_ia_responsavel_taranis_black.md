# Política Corporativa de Inteligência Artificial Responsável — Taranis Black (Rota Zero — Etapa 3)

**Projeto:** Challenge ONE G11 — AI for Business  
**Empresa Simulada:** Taranis Black  
**Responsável:** Lídi Moura  
**Data:** 08/11/2026 | **Versão:** 1.0 (MVP Executivo)  

---

## 1. Objetivo e Escopo da Política

Estabelecer diretrizes claras, auditáveis e em total conformidade com a **Lei Geral de Proteção de Dados (LGPD — Lei nº 13.709/2018)** para o uso seguro, ético e responsável de ferramentas de Inteligência Artificial Generativa, Preditiva e Tradicional (incluindo ChatGPT, Google Gemini, Claude, Antigravity, Google Colab e assistentes internos) por todas as pessoas colaboradoras, lideranças e prestadores de serviço da **Taranis Black**.

---

## 2. Diretrizes Práticas de Uso: O Que PODE vs. O Que NÃO PODE

| Dimensão | ✅ O QUE PODE (Usos Permitidos e Incentivados) | 🚫 O QUE NÃO PODE (Usos Estritamente Proibidos) |
| :--- | :--- | :--- |
| **Treinamento de Liderança e RH** | • Praticar conversas difíceis e feedbacks utilizando **personas 100% fictícias** no Simulador SBI homologado pelo RH;<br>• Solicitar sugestões de estruturação comunicativa no modelo Situação-Comportamento-Impacto para situações descritas de forma genérica e anônima;<br>• Criar roteiros de onboarding, pautas de reuniões 1:1 e materiais educativos. | • **Proibido automatizar decisões de RH:** jamais usar IA para decidir ou recomendar contratação, promoção, reajuste salarial, advertência, punição ou desligamento de qualquer pessoa;<br>• Proibido utilizar o desempenho do gestor dentro do Simulador SBI como nota de avaliação formal ou critério punitivo;<br>• Proibido usar o simulador em substituição à mediação humana presencial em casos de assédio, discriminação ou saúde mental. |
| **Dados Pessoais, Privacidade e Segredos (LGPD)** | • Processar bases de People Analytics **somente após anonimização e minimização** (remoção de nomes, e-mails, CPFs e salários individuais na Camada Prata);<br>• Trabalhar com indicadores estatísticos agregados por departamento ou temas gerais de clima;<br>• Consultar catálogos públicos de produtos (*ErgoPro, SmartDesk, Silence*) e normas técnicas (NR-17). | • **Zero PII em LLMs externos:** proibido colar nomes completos, CPFs, e-mails, telefones, endereços, salários individuais, atestados médicos, avaliações nominais ou transcrições identificáveis de entrevistas de saída em prompts de IA;<br>• **Zero Segredos Técnicos/Comerciais:** proibido inserir senhas, chaves de API, tokens, JWTs, arquivos `.env`, contratos confidenciais de clientes B2B ou dados bancários. |
| **Comercial, Marketing, Finanças e Operações** | • Treinar contorno de objeções B2B com base no catálogo oficial;<br>• Adaptar textos-semente para redes sociais seguindo o Guia de Tom de Voz da Taranis Black, com revisão humana final;<br>• Apoiar análises agregadas de orçamento (DRE) e mapeamento de fluxos operacionais (SIPOC/Ishikawa). | • Proibido disparar comunicações automatizadas a clientes, candidatos ou colaboradores sem revisão humana prévia e sem transparência;<br>• Proibido aprovar ou reprovar crédito de clientes B2B ou alterar registros financeiros no ERP de forma autônoma por IA sem validação da Controladoria;<br>• Proibido apresentar estimativas ou hipóteses geradas por IA como fatos causais comprovados sem verificação na base oficial. |

---

## 3. Mapeamento de Riscos de Viés, Privacidade (LGPD) e Controles de Mitigação

| Categoria de Risco | Descrição do Risco Identificado na Taranis Black | Princípio / Artigo LGPD Relacionado | Controles Técnicos e Organizacionais de Mitigação |
| :--- | :--- | :--- | :--- |
| **1. Violação de Privacidade e Reidentificação Indireta** | Em departamentos menores (ex.: *Gente e Cultura* com 15 pessoas ou *Marketing* com 25) ou em amostras qualitativas pequenas (`n = 14`), cruzar cargo, tempo de casa e comentário aberto pode permitir identificar o autor mesmo sem o nome. | **Art. 6º, I, II e III (Finalidade, Adequação e Necessidade / Minimização)** e **Art. 12 (Anonimização)** | • **Descarte na origem (Camada Prata):** remoção programática de `Nome` e `Salário Mensal` antes das análises;<br>• **Regra de Corte Mínimo (*k-anonymity*):** proibição de reportar cruzamentos qualitativos de grupos com menos de 5 integrantes;<br>• Consolidação temática agregada em vez de exposição de relatos individuais. |
| **2. Viés Algorítmico e Estereotipação em RH** | LLMs podem reproduzir vieses de gênero, idade, região ou estilo comunicativo ao simular personas ou avaliar o tom de um gestor, ou induzir viés de confirmação na leitura de entrevistas de saída. | **Art. 6º, IX (Não Discriminação)** | • **Rubrica Determinística e Transparente:** o Simulador SBI avalia estritamente os 5 elementos objetivos (Situação, Comportamento observável, Impacto, Tom respeitoso e Próximo Passo), vedando julgamentos de personalidade;<br>• Revisão diversa das personas pelo Comitê de IA para evitar caricaturas discriminatórias. |
| **3. Decisão Automatizada Lesiva ao Trabalhador** | Risco de gestores tentarem usar pontuações de IA, análises de sentimento ou modelos preditivos futuros para justificar demissões ou bloqueio de promoções nos primeiros 90 dias. | **Art. 20 da LGPD (Direito à revisão de decisões tomadas unicamente com base em tratamento automatizado)** | • **Supervisão Humana Obrigatória (*Human-in-the-Loop*):** toda decisão sobre carreira, retenção ou desligamento exige parecer humano fundamentado de Gestor + BP de RH;<br>• Canal aberto de contestação e revisão humana para qualquer recomendação apoiada por sistemas analíticos. |
| **4. Alucinação e Distorção de Dados Executivos** | Risco de um LLM inventar percentuais de turnover ou confundir métricas (ex.: misturar turnover sobre a base total com proporção sobre desligados). | **Art. 6º, IV e V (Livre Acesso e Qualidade dos Dados / Exatidão)** | • **Separação de Tarefas:** cálculos quantitativos são executados exclusivamente via código determinístico auditável (Python/Pandas no Colab), cabendo à IA generativa apenas apoiar a síntese textual após validação humana dos números. |
| **5. Vazamento de Credenciais e Treinamento Externo** | Uso de contas gratuitas não corporativas onde os dados inseridos nos prompts possam ser usados para treinar modelos públicos de terceiros. | **Art. 46 da LGPD (Segurança e Prevenção)** | • Uso exclusivo de ambientes homologados com opt-out de treinamento externo;<br>• Diretriz de **Tolerância Zero a Hardcoding** (uso de `.gitignore` bloqueando `.xlsx`, `.csv` e `.env`). |

---

## 4. Comitê de Governança de IA e Rituais de Auditoria

Para garantir que esta política não seja apenas declaratória, a Taranis Black institui o **Comitê Multidisciplinar de Governança de IA e Ética**:

### 4.1. Composição do Comitê
1. **Patrocínio Executivo (Sponsor):** CEO da Taranis Black (autoridade final sobre diretrizes estratégicas, investimentos e aprovação de escopo).
2. **Liderança de Pessoas (Guardião Cultural e HITL):** Liderança de Gente & Cultura / BP Sênior de RH e Analista de People Analytics.
3. **Conformidade Legal e Privacidade:** Encarregado de Proteção de Dados (**DPO / Jurídico**), responsável pela conformidade contínua com a LGPD.
4. **Segurança e Infraestrutura Técnica:** Liderança de TI / Engenharia de Dados, responsável pelo controle de acessos (RBAC), homologação de ferramentas e segurança de repositórios.
5. **Representação das Áreas de Negócio:** 1 representante rotativo das lideranças operacionais (Comercial B2B, Suporte ao Cliente, Operações/Logística ou Finanças) para garantir aderência prática.

### 4.2. Cadência dos Rituais de Auditoria e Monitoramento

| Ritual de Governança | Frequência | Responsáveis | Escopo e Entregáveis de Auditoria |
| :--- | :---: | :--- | :--- |
| **1. Auditoria Operacional do Piloto (Logs & Prompts)** | **Mensal** *(durante os primeiros 90 dias)* | People Analytics + BP de RH + TI | • Verificação amostral de sessões do Simulador SBI para confirmar ausência de inserção de dados pessoais reais;<br>• Calibração da rubrica SBI e revisão de eventuais falhas ou alucinações reportadas pelos gestores;<br>• Checagem do registro de prompts (ferramenta, versão, finalidade e revisor humano). |
| **2. Auditoria de Conformidade LGPD, Vieses e Clima** | **Trimestral** | DPO / Jurídico + Comitê Completo | • Auditoria de privacidade e anonimização nas bases de People Analytics (Camadas Bronze, Prata e Ouro);<br>• Avaliação de equidade e mitigação de vieses nos cenários de treinamento e relatórios de clima;<br>• Revisão de incidentes ou solicitações de contestação humana (Art. 20 LGPD). |
| **3. Revisão Estratégica da Política e Catálogo de IA** | **Semestral** | CEO + Comitê Completo | • Atualização da lista de ferramentas homologadas e níveis de acesso por função (RBAC);<br>• Avaliação das métricas de impacto, adoção e maturidade cultural;<br>• Aprovação de novos casos de uso do roadmap (ex.: expansão do Onboarding Inteligente RAG e automações interdepartamentais). |
