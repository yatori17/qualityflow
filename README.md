# QualityFlow 🚀
> **Projeto MVP para a Sprint de Gestão Ágil de Projetos e Produtos**

O **QualityFlow** é uma plataforma centralizadora de métricas de qualidade de software projetada para equipes ágeis que sofrem com o acúmulo de débito técnico e falta de visibilidade sobre a saúde do código. 

Inspirado em conceitos de ferramentas como o SonarQube, o QualityFlow se diferencia por ser uma solução *lightweight* (leve). Em vez de realizar varreduras pesadas no código-fonte, ele atua como um consolidador inteligente: recebe relatórios estruturados (JSON/XML) gerados pelas próprias ferramentas de automação da equipe (como JUnit, Mockito e JMeter) via API e os transforma em um painel visual direto, limpo e de rápida configuração.

---

## 👥 1. Cenário de Negócio Hipotético

### Stakeholders, Clientes e Usuários
*   **Stakeholders:** Diretores de Tecnologia (CTOs), Engenheiros Líderes e investidores focados em eficiência operacional.
*   **Clientes:** Empresas de tecnologia (B2B) de médio e pequeno porte que buscam reduzir o tempo gasto com refatorações e manutenções corretivas.
*   **Usuários:** Desenvolvedores de Software, Analistas de QA e Scrum Masters que necessitam de dados consolidados para guiar as reuniões de Retrospectiva e Planejamento de Sprint.

### 👥 Time Scrum Enxuto
A equipe foi dimensionada com o mínimo de integrantes necessários para garantir a entrega do MVP com máxima qualidade:
1.  **Product Owner (PO):** Responsável por definir os requisitos de negócio e priorizar as métricas de maior impacto.
2.  **Scrum Master (SM):** Facilitador do processo ágil, focado na remoção de impedimentos e blindagem do time.
3.  **Dev Backend (Foco em Integração):** Especialista em APIs para construir os endpoints que recebem e processam os dados de qualidade.
4.  **Dev Frontend (UI/UX):** Responsável por construir o dashboard visual de alta legibilidade.
5.  **Analista de QA / DevOps:** Focado na qualidade da plataforma e na automação das esteiras de verificação.

---

## 🎯 2. Escopo do MVP (Mínimo Viável)

A estratégia adotada na nossa *Lean Inception* delimitou claramente as fronteiras do produto para este primeiro lançamento:

| 🟩 Fica no MVP (Ondas 1 e 2) | 🟥 Próximos Incrementos (Futuro) |
| :--- | :--- |
| Tela de Login e Tela de Seleção de Projetos. | Gráficos de linha históricos com tendências de Sprints passadas. |
| API pública (`POST /v1/metrics`) para recepção de payloads de teste. | Integração nativa e via plugins com GitHub Actions e Jenkins. |
| Processadores (Parsers) automatizados para JUnit e JMeter. | Filtros avançados de busca por intervalo customizado de datas. |
| Dashboard Web com exibição de Cobertura, Bugs Críticos e Performance. | Sistema de alertas automatizados via Slack ou Microsoft Teams. |
| Geração de token de autenticação simples por projeto. | Relatórios preditivos de evolução de débito técnico usando IA. |

---

## 📋 3. Acordos de Trabalho (DoR e DoD)

### 🟩 Definition of Ready (DoR)
Para que uma História de Usuário seja selecionada para a Sprint, ela precisa obrigatoriamente cumprir:
*   Descrição clara no formato padrão (*Como... Quero... Para...*).
*   Critérios de aceitação definidos utilizando a sintaxe BDD (*Gherkin*).
*   Estimativa de esforço definida coletivamente em *Story Points* (Fibonacci).
*   Wireframe de baixa ou média fidelidade anexado à tarefa (se houver componente visual).
*   Ausência de dependências ou bloqueios técnicos externos.

### 🟥 Definition of Done (DoD)
Uma entrega só é considerada concluída ("Pronta") se atender a todos os critérios:
*   Código revisado via *Pull Request* por pelo menos um par de desenvolvimento.
*   Cobertura mínima de 80% em testes unitários automatizados.
*   Autenticação e rotas protegidas via Spring Security através de tokens de projeto.
*   **Requisito Não Funcional (Performance):** O tempo de resposta da API do dashboard para renderização dos dados deve ser menor que **400ms**.
*   Validação final e aceite funcional realizado pelo Product Owner em ambiente de staging.

---

## 📦 4. Estrutura do Repositório

Este repositório está organizado estritamente de acordo com as diretrizes da avaliação:

*   `/wireframes`: Contém as telas do protótipo de baixa fidelidade exportadas do Figma.
*   `canvas-url.txt`: Arquivo com o link público do board do Miro (Lean Inception + MVP Canvas).
*   `product-backlog.pdf`: Relatório completo extraído do JIRA contendo Épicos, Features e Histórias.
*   `sprint-backlog.pdf`: Planejamento detalhado da Sprint 1 extraído do JIRA com estimativas e critérios.
*   `video-showcase.mp4`: Vídeo demonstrativo da entrega (Showcase de 2 a 4 minutos).

---
*Desenvolvido como parte do portfólio acadêmico de Gestão Ágil e Engenharia de Requisitos.*# QualityFlow 🚀