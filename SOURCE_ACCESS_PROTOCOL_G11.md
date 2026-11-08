# Protocolo de acesso às fontes — G11 Rota 3

## Regra principal

O Antigravity não deve presumir acesso ao Google Workspace, aos NotebookLM ou às fontes privadas da Lídi. Ele só pode usar materiais que estejam: (1) anexados ao contexto da execução; (2) presentes no repositório; (3) publicados como link aberto; ou (4) explicitamente autorizados e acessíveis pela integração da ferramenta.

## Fontes autorizadas para o MVP

1. `Challenge G11 - Taranis Black.txt`.
2. `00_INDICE_E_GUIA_DO_KIT_DE_DADOS.md`.
3. `04_Base_Colaboradores_People_Analytics.xlsx`, somente em ambiente local/Colab autorizado; nunca versionar.
4. `00_BASE_CHALLENGE_R0_R3.md`.
5. Template oficial da Rota 3: `https://docs.google.com/document/d/1tNPwSv6YateSQ0gUa_kCHB0v10v5i2ALLW5VcjUGA5M/edit`.
6. Notebook Colab do projeto.
7. Links públicos de NotebookLM fornecidos pela CEO, quando a ferramenta conseguir acessá-los.
8. Materiais do Hub OS NEXUS e hub-os-guIA apenas como governança e mentoria.

## Como disponibilizar NotebookLM ao Antigravity

Não basta mencionar que os notebooks existem. Para garantir reprodutibilidade, usar uma destas opções:

### Opção A — links públicos

Fornecer ao Antigravity os URLs abertos dos notebooks e instruir: “consulte somente o conteúdo acessível por estes links; não invente conteúdo não disponível”.

### Opção B — exportação controlada

Exportar as transcrições ou resumos essenciais para PDF/Markdown/TXT e colocar no repositório ou anexar à execução. Preservar nome da fonte, curso, data e classificação: fato, hipótese, aprendizado, decisão ou evidência.

### Opção C — material já compartilhado

Usar os arquivos do projeto Manus, que já incluem o enunciado, o kit de dados e materiais de apoio. Esta é a opção recomendada para a entrega urgente, pois reduz dependência de integrações externas.

## O que o Antigravity não deve fazer

- Não pedir senha, token ou credencial da Lídi.
- Não solicitar acesso amplo ao Drive quando um link de visualização for suficiente.
- Não assumir que NotebookLM é fonte da verdade do Challenge.
- Não copiar transcrições integrais sem necessidade.
- Não incluir arquivos `.env`, tokens, JWTs ou dados individuais no repositório.
- Não editar o template original; trabalhar em uma cópia autorizada.
- Não enviar o link à Alura.
- Não alterar permissões externas sem aprovação da CEO.

## Campos obrigatórios do template oficial

### Rota Zero

- Resumo Executivo.
- AI Canvas e mapeamento de oportunidades.
- Mínimo de três casos de uso.
- Classificação por tipo de IA: generativa, preditiva ou tradicional.
- Supervisão humana.
- Matriz Esforço × Impacto.
- Métricas de sucesso.
- Plano de mudança.
- Política de IA Responsável.
- Riscos e LGPD.
- Comitê e auditoria.

### Rota 3 — obrigatório

- Três ou mais personas de colaboradores.
- Prompt de sistema completo.
- Exemplo de sessão aplicando Situação, Comportamento e Impacto.
- Avaliação da eficácia e melhorias no prompt.

### Rota 3 — opcional recomendada

- Métricas calculadas.
- Hipóteses diagnósticas geradas com IA.
- Recomendações de ação.
- Links e prints das análises.

### Anexo de evidências

Cada linha deve conter:

- artefato;
- descrição;
- link;
- print/captura;
- nota de uso.

## Registro das ferramentas

No relatório, declarar com transparência:

- **Google Docs/Drive:** documento final e anexos.
- **Google Colab/Python:** análise agregada e gráficos.
- **Antigravity:** execução técnica, documentação e apoio à construção dos artefatos.
- **Hub OS NEXUS:** autoridade arquitetural, segurança, governança e DEVLOG.
- **hub-os-guIA:** mentoria, organização de fontes, QA, STAR e portfólio.
- **NotebookLM:** estudo e consulta de materiais, quando acessível.
- **Canva:** AI Canvas, matriz e roadmap visuais, se utilizado.

## Critério de confiança

Se uma fonte não puder ser acessada, registrar “não acessível nesta execução” e seguir com as fontes oficiais do projeto. Nunca preencher lacunas por suposição silenciosa.
