# EduCode

Sistema de gestão educacional para instituições de pequeno e médio porte.

## Sobre o Projeto

O EduCode é uma plataforma digital desenvolvida no contexto do **Projeto Integrador** do curso de **Engenharia de Software** da **UniEVANGÉLICA**. O sistema tem como objetivo modernizar a administração de instituições de ensino, substituindo processos manuais e fragmentados por um ambiente integrado para controle de matrículas, frequência, comunicação institucional e geração de relatórios.

Este repositório foi criado durante o **2º período (Fase 02)** para abrigar o código-fonte do projeto. A implementação será realizada progressivamente a partir dos períodos seguintes, conforme as diretrizes do Projeto Integrador.

# EduCode

> **Projeto Integrador — Engenharia de Software (UniEVANGÉLICA)**  
> **Fase Atual:** Documentação e Prototipação (3º Período)

## 1. Objetivo

O **EduCode** é uma plataforma digital centralizada desenvolvida para modernizar a gestão administrativa e pedagógica de instituições educacionais de pequeno e médio porte, com foco prioritário em organizações do terceiro setor e projetos socioeducativos com estrutura administrativa reduzida e recursos limitados (cenário baseado no Projeto Semear, instituição sem fins lucrativos que atende crianças e adolescentes no contraturno escolar).

### Problemas que o Projeto Resolve
* **Dependência de Processos Manuais e Físicos:** Substituição definitiva do uso de registros em papel, cadernos e planilhas físicas isoladas para gestão de informações críticas (como matrículas, controle de frequência e notas), eliminando a vulnerabilidade e ineficiência dos métodos analógicos.
* **Ineficiência Operacional e Risco de Perda de Dados:** Mitigação do alto risco de perda ou extravio de documentos físicos e eliminação da lentidão na consolidação de históricos escolares e relatórios de desempenho, automatizando rotinas operacionais e eliminando duplicidade de esforços.
* **Fragmentação das Informações e Comunicação Informal:** Solução para a dispersão de dados em múltiplos locais e a dependência de canais informais (como conversas de WhatsApp e recados verbais), estabelecendo um canal institucional centralizado para envio de avisos, consulta de rotinas e acompanhamento da vida escolar.
* **Instabilidade e Lentidão em Plataformas Existentes:** Resposta às dores relatadas por usuários em relação a sistemas legados em uso no mercado (como o SIAP, frequentemente apontado com problemas de lentidão acentuada, sobrecarga e indisponibilidade em momentos críticos de uso).

### Público-Alvo
* **Coordenação Pedagógica e Administrativa:** Gestores que realizam matrículas, modulam salas, gerenciam a lista de espera, administram registros de doações e necessitam de visão consolidada dos dados institucionais por meio de dashboards e relatórios oficiais.
* **Professores (Corpo Docente):** Educadores que realizam o lançamento diário de presenças/faltas, o registro de notas e avaliações por disciplina/turma e a publicação de avisos direcionados aos alunos.
* **Responsáveis e Alunos:** Familiares que necessitam de acesso autônomo, direto e transparente à rotina dos dependentes (frequência, notas, comunicados/avisos e acompanhamento de posição na lista de espera), sem dependência de intermediação manual constante da instituição.

## 2. Escopo

O escopo do projeto está delimitado em conformidade com os requisitos levantados (RF-001 a RF-022, RNF-001 a RNF-010 e RNE-001 a RNE-008) e com o estágio pedagógico atual do curso.

### Contemplado nesta fase (Documentação e Prototipação)
* **Levantamento e Especificação de Requisitos:**
  * Requisitos Funcionais (RF-001 a RF-022): controle de acesso e perfis, gestão de matrículas, cadastro de contatos de responsáveis, relatórios, lista de espera, módulo de doações, mural de avisos, gestão de salas, atividades diárias e extracurriculares e painel consolidado do aluno.
  * Requisitos Não Funcionais (RNF-001 a RNF-010): foco em usabilidade e redução de cliques (máximo de 2 níveis de navegação), conformidade com a LGPD, segurança de acesso por perfil, responsividade e disponibilidade mínima de 99%.
  * Regras de Negócio (RNE-001 a RNE-008): obrigatoriedade de matrícula presencial prévia, unicidade de cadastro por aluno, permissão restrita da coordenação para aprovação de lista de espera e segregação do módulo de doações.
* **Pesquisa com Usuários:** Elaboração, aplicação junto a 12 participantes (6 professores, 3 coordenadores e 3 responsáveis) e análise dos resultados convertidos em requisitos reais.
* **Design e Experiência do Usuário (UI/UX):**
  * Mapeamento de fluxos de navegação segmentados por perfil (Coordenação, Professor e Responsável).
  * Wireframes de baixa fidelidade e telas de média fidelidade (Fases 01 e 02) cobrindo Login, Dashboards, Matrículas, Lista de Espera, Avisos, Faltas, Relatórios, Salas, Atividades e Doações.
  * Protótipo interativo e navegável estruturado no Figma.
* **Modelagem Conceitual:** Diagrama de Casos de Uso (UML) formalizando os limites do sistema e os casos de uso de cada ator.
* **Gestão Ágil e Repositórios:** Definição de sprints (Sprints 1 e 2 do 2º período) e estruturação dos repositórios oficiais.

### Fora do escopo nesta fase
* **Implementação de Código Executável:** Desenvolvimento de código de frontend (HTML/CSS/JS/frameworks), backend (APIs, serviços, controladores) e integração funcional entre camadas (planejados para os períodos seguintes da graduação).
* **Banco de Dados Físico Operacional:** Criação de schemas físicos em SGBD em produção e scripts operacionais (a modelagem de dados detalhada inicia-se no 3º período).
* **Executáveis, Build e Deploy:** Não há pacotes instaláveis, empacotamento, containerização ou deploy em nuvem nesta fase.
* **Integrações Tecnológicas Externas Reais:** Disparo em tempo real de notificações push para smartphones ou integração bancária com gateway de pagamento para doações.
* **Testes Automatizados de Software:** Execução de testes unitários ou de integração sobre código-fonte (previstos para a etapa de qualidade no 7º período).

## 3. Time e papéis

A composição da equipe de desenvolvimento do projeto é apresentada na tabela abaixo. Os papéis Scrum formais estão alinhados com a estrutura ágil do projeto e com o arquivo `docs/time-agil.md`:

| Nome Completo | Papel Scrum | Atribuição no Projeto Integrador |
| :--- | :--- | :--- |
| **Bruno Alexandre** | A definir (Product Owner) | Liderança de Equipe e Pesquisa de Mercado |
| **Davi Isaac** | A definir (Developer) | Design de Interface (UI/UX) e Prototipação |
| **Lucas Felipe** | A definir (Scrum Master) | Documentação Técnica, Validação de Conteúdo e Análise de Mercado |
| **Natália Estevão** | A definir (Developer) | Engenharia de Requisitos e Apoio Documental |

> **Orientação Acadêmica:**
> * Prof. Eduardo Dias Pereira (Orientador Principal)
> * Prof. Jeferson Silva Araújo (Orientador Secundário)

## 4. Como executar / Como acessar

> **Aviso:** Não existe implementação executável nem código-fonte funcional nesta fase do projeto. O sistema está restrito às fases de levantamento de requisitos, especificação documental e prototipação. Dessa forma, não existem procedimentos de instalação, compilação de arquivos ou comandos de execução em terminal (`npm install`, `docker`, `python main.py`, etc.).

Os artefatos e protótipos oficiais do projeto podem ser consultados através dos seguintes links e locais:

1. **Repositório de Protótipos e Wireframes (GitHub):**
   * Link: [https://github.com/Lucas-Felipe17/educode-prototipo](https://github.com/Lucas-Felipe17/educode-prototipo)
   * Artefatos disponíveis:
     * Diretório `WIREFRAMES/`: Wireframes de baixa fidelidade (`Atividades.png`, `Avisos.png`, `Faltas.png`, `Lista de espera.png`, `Matriculas.png`) e documentação explicativa `wireframes.md`.
     * Arquivo `figma-link.txt`: Arquivo com referências para o protótipo e fluxo no Figma.
2. **Repositório Oficial de Código (GitHub):**
   * Link: [https://github.com/Lucas-Felipe17/educode-codigo](https://github.com/Lucas-Felipe17/educode-codigo)
   * Repositório destinado à futura implementação do código-fonte (atualmente contendo a parametrização inicial e este `README.md`).
3. **Questionário da Pesquisa com Usuários (Google Forms):**
   * Link: [Questionário de Pesquisa EduCode](https://docs.google.com/forms/d/e/1FAIpQLSfAPIaCKr-F7dOPIfSnrt1S9xXXXWGio1ttif5IBP_WaHhYtw/viewform?usp=sharing&ouid=100170045955189046748)
4. **Protótipo Interativo no Figma:**
   * Link: [Figma] (https://www.figma.com/design/NJ75xlvxPkE1fKGcYK05a5/PI_PROT%C3%93TIPO?node-id=0-1&t=6lzJsraY2jJp7ZMl-1).
