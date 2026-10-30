# Time Ágil — EduCode

## Papéis do time

Nesta seção, definimos as responsabilidades de cada integrante do grupo para a fase atual de documentação e prototipação do Projeto Integrador.
As informações devem ser idênticas às cadastradas pelo Integrante 1 no README.

## Definition of Ready

Para que uma atividade possa sair do fluxo inicial e entrar em DOING (Em andamento), ela deve cumprir as seguintes condições verificáveis do processo real do grupo:

- Objetivo da atividade definido.
- Escopo compreendido pelo integrante responsável.
- Informações necessárias disponíveis para execução.
- Critérios de aceitação definidos.
- Prioridade definida.
- Responsável pela atividade identificado, quando aplicável.

## Definition of Done

Para que uma atividade seja considerada efetivamente concluída no contexto atual de documentação e prototipação, ela deve cumprir os seguintes critérios objetivos:

- [ ] Todos os critérios de aceitação da issue foram atendidos
- [ ] O PR aponta a issue que resolve (Closes #número)
- [ ] Outro integrante revisou e aprovou o PR
- [ ] A documentação afetada foi atualizada
- [ ] Não há conflitos com a branch main

## Matriz de stakeholders

### Identificação de stakeholders

| Nº | Stakeholder (nome ou grupo) | Função no projeto | Interno ou externo | Interesse | Poder |
| --- | --- | --- | --- | --- | --- |
| 1 | Coordenação pedagógica | Usuário-chave e validador das regras de negócio (matrículas, relatórios e lista de espera). | Externo | Alto | Médio |
| 2 | Professores | Usuários operacionais de faltas, notas e avisos. Validam usabilidade e fluxos pedagógicos. | Externo | Alto | Médio |
| 3 | Responsáveis | Usuários finais de acompanhamento do aluno e canal de comunicação. Validam linguagem e acesso. | Externo | Alto | Baixo |
| 4 | Alunos | Usuários finais de avisos, atividades e notas, quando aplicável. Recebem o resultado. | Externo | Médio | Baixo |
| 5 | Agência Nacional de Proteção de Dados (ANPD) | Órgão regulador e fiscalizador da LGPD. Exige adequações e fiscaliza o tratamento de dados. | Externo | Baixo | Alto |
| 6 | Orientadores do projeto | Orientam, avaliam e aprovam entregas acadêmicas. | Interno | Alto | Alto |
| 7 | Equipe do Projeto | Executa design, requisitos, prototipação e documentação. | Interno | Alto | Alto |
| 8 | Coordenação do Curso | Define diretrizes, prazos e avaliação do PI. Fiscaliza conformidade acadêmica. | Interno | Médio | Alto |

### Matriz poder × interesse

O critério Médio é tratado como baixo para posicionar o stakeholder no quadrante.

| Quadrante | Estratégia | Stakeholders (Nº e nome) |
| --- | --- | --- |
| Alto poder · alto interesse | Gerenciar de perto | 6. Orientadores; 7. Equipe do Projeto |
| Alto poder · baixo interesse | Manter satisfeito | 5. ANPD; 8. Coordenação do Curso |
| Baixo poder · alto interesse | Manter informado | 1. Coordenação pedagógica; 2. Professores; 3. Responsáveis |
| Baixo poder · baixo interesse | Monitorar | 4. Alunos |

### Justificativa dos níveis Médio

- **1 Coordenação pedagógica.** Poder Médio: valida requisitos e regras de negócio, mas não aprova escopo nem entregas do PI, que ficam com os orientadores.
- **2 Professores.** Poder Médio: influenciam os requisitos e a adoção pelo uso diário, mas não aprovam escopo ou entregas formais.
- **4 Alunos.** Interesse Médio: são afetados por avisos, atividades e notas, mas têm participação limitada nas decisões do projeto.
- **8 Coordenação do Curso.** Interesse Médio: não acompanha o detalhe funcional no dia a dia, mas define normas, prazos e avaliação.

## Plano de comunicação

**Marco:** conclusão de cada fase do PI (Fase 01, 02, 03).

**Período:** semestre letivo.

| Stakeholders (Nº) | O que comunicar | Evento do Scrum ou canal | Frequência | Responsável no time |
| --- | --- | --- | --- | --- |
| 7 | Objetivo da sprint, itens priorizados e critérios de aceitação | Sprint Planning | Quinzenal (início da sprint) | Product Owner |
| 7 | Progresso, impedimentos e dependências | Daily Scrum | Diária | Developers |
| 6, 7 | Demonstração do incremento, decisões de prioridade, escopo e riscos | Sprint Review | Quinzenal | Product Owner |
| 7 | Lições aprendidas e melhorias do processo | Sprint Retrospective | Quinzenal | Scrum Master |
| 1, 2, 3, 4 | Demonstração do incremento e validação das telas e fluxos | Sprint Review (a última do período) | Uma vez por período | Product Owner |
| 1, 2, 3, 4 | Perguntas para definir escopo e validar ideias, com retorno sobre o que foi decidido | Questionário | Uma vez por período, no primeiro marco | Product Owner |
| 1, 2, 3 | Dúvidas pontuais sobre processos e rotinas da instituição | Mensagem curta (WhatsApp ou e-mail) | Sob demanda | Product Owner |
| 5 | Resumo das medidas de conformidade com a LGPD, tratamento de dados, auditoria e mudanças relevantes de segurança | Resumo escrito | A cada marco | Product Owner |
| 8 | Marcos entregues, prazos cumpridos e riscos de conformidade acadêmica | AVA (canal) | A cada marco | Product Owner |

## Quadro e limite de WIP

**Quadro:** [GitHub Projects do time](https://github.com/users/Lucas-Felipe17/projects/1)

### Colunas e mapeamento

| Coluna      | Etapa | Regra de entrada                           |
| ----------- | ----- | ------------------------------------------ |
| Backlog     | TO-DO | Issue criada pelo template, com MoSCoW     |
| Ready       | TO-DO | Atende à Definition of Ready               |
| In-progress | DOING | Dupla puxa a issue de Ready, dentro do WIP |
| In-review   | DOING | PR aberto no template, com `Closes #n`     |
| Done        | DONE  | Atende à Definition of Done (checklist)    |

### Limite de WIP do DOING

**2 issues simultâneas**, somando as colunas In-progress e In-review.

### Justificativa

O time tem 4 integrantes e trabalha em duplas (pareamento), com 2 pessoas por
issue. Com 2 duplas, o máximo de trabalho em paralelo sem dividir a atenção de
ninguém é 2 issues, ou seja, WIP = nº de integrantes ÷ 2. Um limite maior
obrigaria alguém a atuar em duas issues ao mesmo tempo.

Como In-review conta no limite, uma dupla com PR aguardando revisão não inicia
outra issue. Ela ajuda a revisar ou concluir o que está em andamento,
priorizando terminar antes de começar.

### Regra de operação

- Ao atingir o limite, nenhuma issue é puxada de Ready.
- A revisão do PR é feita preferencialmente pela outra dupla.
- Se uma issue ficar bloqueada, o time resolve o bloqueio na daily (ou na
  revisão semanal) em vez de abrir uma nova issue.

## Declaração de uso de IA

O time usou ferramentas de IA generativa neste projeto.

### Ferramentas e finalidade

| Ferramenta | Para que foi usada | Onde apareceu no repositório |
| --- | --- | --- |
| Claude | Formatação e estruturação dos templates de PR, e ISSUES, de acordo com o conteúdo proposto pelos integrantes | .github/pull_request_template.md, .github/ISSUES_TEMPLATE/bugs, .github/ISSUES_TEMPLATE/funcionalidade |
| DeepSeek | Formatação da estrutura em Markdown de readme.md | readme.md |
| ChatGPT | Sugestão de estrutura e formatação em Markdown de docs/time-agil.md | docs/time-agil.md |

### O que o time revisou ou mudou

- O conteúdo da matriz de stakeholders e do plano de comunicação veio da Atividade da Aula 11, da disciplina de Gestão Ágil de projetos, feita pelo grupo; a IA só ajudou na formatação
- O limite de WIP e a justificativa foram definidos pelo grupo a partir do tamanho do time; a IA sugeriu uma redação, que foi ajustada.
- verificamos que a DoR e a DoD do documento batem com o checklist do template de PR

### Limites do uso

- Nenhum dado pessoal ou sensível foi enviado às ferramentas
- O time é responsável pelo conteúdo entregue
