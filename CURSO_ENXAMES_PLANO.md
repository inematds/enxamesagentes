# CURSO COMPLETO: Enxames de Agentes de IA

> **Domine a construcao de sistemas multiagentes inteligentes**
> **Versao:** 1.0 | **Data:** 2026-03-19

---

## VISAO GERAL DO CURSO

| Item | Valor |
|------|-------|
| Nome | Enxames de Agentes de IA |
| Emoji | `🐝` |
| Total de Trilhas | 4 |
| Total de Modulos | 32 |
| Topicos por Modulo | 6-8 |
| Total Estimado de Topicos | ~220 |

### Tema Central

Sistemas multiagentes (swarms) permitem que equipes de IAs especializadas colaborem para resolver problemas complexos. Em vez de sobrecarregar um unico modelo com todas as tarefas, um orquestrador coordena subagentes especializados que trabalham em paralelo — como uma cozinha de restaurante com chef, sommelier, pasteleiro e maitre, cada um fazendo o que melhor sabe.

### Publico-Alvo

- Desenvolvedores e entusiastas de IA que querem ir alem do uso basico de LLMs
- Profissionais que desejam construir sistemas de automacao mais robustos
- Quem ja usa ferramentas como OpenCode, Claude Code, ou similares

### Conteudo Fonte Disponivel

| Arquivo | Descricao |
|---------|-----------|
| `doc/enxamesdeagentes.txt` | Introducao + guia espanhol OMO + transcricao completa da videoaula |
| `doc/guia-oh-my-openagent-pt.md` | Guia completo em PT-BR (instalacao, 3 modos, 7 agentes, configuracao) |
| `doc/swarm-avancado-opencode.md` | Resumo estruturado da aula "Swarm avancado no OpenCode" — fluxo, conselhos-chave, resultado |
| [opencode-swarm](https://github.com/zaxbysauce/opencode-swarm) | 828 commits, 18 design decisions, 9 agentes, gates de QA, sistema Curator |

### Ilustracoes Disponíveis

| Arquivo | Descricao | Uso Sugerido |
|---------|-----------|--------------|
| `doc/ChatGPT Image 19...06_27_15.png` | "ENXAME DE AGENTES" — agentes em paralelo, comunicando-se, alcancando objetivos | Hero da pagina index e Trilha 1 |
| `doc/ChatGPT Image 19...06_04_43.png` | Exercito de agentes cyberpunk com olhos azuis | Hero da Trilha 3 (Pratica Avancada) |
| `doc/photo_5035387927072017301_w.jpg` | Diagrama arquitetural completo OMO (sequencial + paralelo + categorias) | Trilha 2 (Tecnicas) — visao geral |
| `doc/photo_5035387927072017302_x.jpg` | "Que es un Swarm de IA?" — Sem swarm vs Com swarm + analogia cozinha | Trilha 1 Modulo 1 — conceito fundamental |
| `doc/photo_5035387927072017303_x.jpg` | Pipeline sequencial OpenCode Swarm (Explorer → SME → Architect → Critic → Coder/Reviewer/Test/Docs) | Trilha 2 Modulo 2 — arquitetura sequencial |
| `doc/photo_5035387927072017304_y.jpg` | oh-my-openagent completo (Sisyphus, categorias, paralelismo, instalacao, modelos) | Trilha 2 Modulo 4 — oh-my-openagent |
| `doc/photo_5035387927072017305_y.jpg` | Comparativo ampliado IA sobrecarregada vs equipe especializada | Trilha 1 Modulo 1 — motivacao |

---

## ESTRUTURA DAS 3 TRILHAS

| Trilha | Nome | Cor | Foco | Modulos |
|--------|------|-----|------|---------|
| T1 | Fundamentos | Emerald (#10B981) | Conceitos, teoria de swarms, agentes basicos, arquiteturas | 8 |
| T2 | Tecnicas | Blue (#3B82F6) | Frameworks, orquestracao, protocolos, implementacao | 8 |
| T3 | Pratica Avancada | Purple (#9b59b6) | Projetos reais, producao, memoria, qualidade, opencode-swarm | 8 |
| T4 | Mao na Massa | Amber (#F59E0B) | Passo a passo completo: do zero ao projeto entregue com swarm | 8 |

---

# TRILHA 1: FUNDAMENTOS (Emerald)

> **Entenda o que sao swarms, por que funcionam e como pensam**
>
> **Ilustracao principal:** `doc/photo_5035387927072017302_x.jpg` (Sem Swarm vs Com Swarm)

## Modulo 1.1 - O que e um Swarm de IA

**Duracao:** ~35 min | **Nivel:** Iniciante

### Topicos:

1. **🤖 Uma IA faz TUDO: o problema**
   - **O que e:** O modelo tradicional onde um unico LLM planeja, programa, revisa, documenta e testa — ficando sobrecarregado
   - **Por que aprender:** Entender a limitacao atual e a motivacao para swarms
   - **Conceitos-chave:** Sobrecarga de contexto, perda de foco, limitacao de tokens

2. **🐝 Swarm = Equipe especializada**
   - **O que e:** Multiplos agentes de IA colaborando, cada um fazendo o que melhor sabe, coordenados por um orquestrador
   - **Por que aprender:** E o paradigma que domina 2026 — 72% dos projetos enterprise ja usam multiagentes
   - **Conceitos-chave:** Orquestrador, subagentes, especializacao, coordenacao

3. **🍳 Analogia da cozinha profissional**
   - **O que e:** Chef coordena, sommelier cuida dos vinhos, pasteleiro dos postres, maitre do servico = Resultado Premium
   - **Por que aprender:** Metafora intuitiva que facilita explicar swarms para qualquer publico
   - **Conceitos-chave:** Divisao de trabalho, coordenacao, resultado coletivo superior

4. **🧬 Origem biologica: inteligencia de enxame**
   - **O que e:** Conceito de Jing Wang e Gerardo Beni (1989): auto-organizacao, descentralizacao, emergencia
   - **Por que aprender:** Base teorica solida para entender por que swarms funcionam
   - **Conceitos-chave:** Colonia de formigas, feromonio (stigmergy), comportamento emergente

5. **📊 Quando usar swarm vs agente unico**
   - **O que e:** Criterios para decidir: complexidade, paralelizacao, especializacao necessaria
   - **Por que aprender:** Nem todo problema precisa de swarm — saber quando e fundamental
   - **Conceitos-chave:** Custo vs beneficio, complexidade, escala do projeto

6. **🚀 Panorama 2026: o mundo agentico**
   - **O que e:** Estado atual do mercado — frameworks, protocolos, adocao enterprise
   - **Por que aprender:** Contexto de mercado para posicionamento profissional
   - **Conceitos-chave:** CrewAI, LangGraph, AutoGen, MCP, A2A, adocao corporativa

### Recursos:
- [Swarm Intelligence - Wikipedia](https://en.wikipedia.org/wiki/Swarm_intelligence)
- [The Agentic AI Future - Tribe AI](https://www.tribe.ai/applied-ai/the-agentic-ai-future-understanding-ai-agents-swarm-intelligence-and-multi-agent-systems)

---

## Modulo 1.2 - Anatomia de um Agente de IA

**Duracao:** ~40 min | **Nivel:** Iniciante

### Topicos:

1. **🧠 De LLM a Agente: a diferenca**
   - **O que e:** Um LLM responde; um agente percebe, raciocina, age e lembra
   - **Por que aprender:** Sem esta distincao, e impossivel projetar swarms eficazes
   - **Conceitos-chave:** Percepcao, raciocinio, acao, memoria

2. **🔄 Loop de raciocinio: ReAct**
   - **O que e:** Padrao Reason + Act — o agente pensa, age, observa resultado, repete
   - **Por que aprender:** E o loop fundamental que faz agentes funcionarem
   - **Conceitos-chave:** Thought, Action, Observation, ciclo iterativo

3. **🛠️ Ferramentas (Tools)**
   - **O que e:** Capacidades que estendem o agente: buscar na web, ler arquivos, executar codigo
   - **Por que aprender:** Agentes sem ferramentas sao apenas chatbots sofisticados
   - **Conceitos-chave:** Function calling, API tools, MCP

4. **💾 Memoria: curta e longa**
   - **O que e:** Contexto da conversa (curta) vs conhecimento persistente (longa)
   - **Por que aprender:** Memoria e o que diferencia agentes uteis de agentes esquecidos
   - **Conceitos-chave:** Context window, RAG, vector store, memoria episodica

5. **📋 Planejamento e decomposicao**
   - **O que e:** Capacidade de dividir tarefas complexas em subtarefas executaveis
   - **Por que aprender:** Essencial para orquestradores de swarm
   - **Conceitos-chave:** Plan-and-Execute, decomposicao hierarquica

6. **🎯 Agente autonomo vs assistente**
   - **O que e:** Graus de autonomia: de chatbot a agente que decide e executa sozinho
   - **Por que aprender:** Escolher o nivel certo de autonomia para cada papel no swarm
   - **Conceitos-chave:** Human-in-the-loop, autonomia total, guardrails

### Recursos:
- [What is a ReAct Agent? - IBM](https://www.ibm.com/think/topics/react-agent)
- [What is Agentic RAG? - IBM](https://www.ibm.com/think/topics/agentic-rag)
- [Comparing ReAct and ReWOO - SPR](https://spr.com/comparing-react-and-rewoo-two-frameworks-for-building-ai-agents-in-generative-ai/)

---

## Modulo 1.3 - Arquiteturas de Swarms

**Duracao:** ~45 min | **Nivel:** Iniciante-Intermediario

### Topicos:

1. **🏗️ Hierarquica (Supervisor/Worker)**
   - **O que e:** Orquestrador central delega para agentes especializados — padrao mais comum
   - **Por que aprender:** E a arquitetura da maioria dos sistemas reais (OpenCode Swarm, CrewAI)
   - **Conceitos-chave:** Hub-and-spoke, delegacao, controle centralizado

2. **🔗 Pipeline sequencial**
   - **O que e:** Cada agente processa uma etapa e passa para o proximo em sequencia
   - **Por que aprender:** Ideal quando ha dependencia entre etapas (ex: codigo → revisao → teste → docs)
   - **Conceitos-chave:** Chain, handoff, dependencia, gated pipeline

3. **🔀 Paralelo (Fan-out/Fan-in)**
   - **O que e:** Multiplos agentes trabalham simultaneamente em tarefas independentes
   - **Por que aprender:** Maximiza velocidade quando tarefas nao dependem umas das outras
   - **Conceitos-chave:** Concorrencia, merge de resultados, zonas seguras

4. **🕸️ Peer Mesh (descentralizado)**
   - **O que e:** Agentes colaboram diretamente sem controle central
   - **Por que aprender:** Alternativa resiliente para cenarios dinamicos
   - **Conceitos-chave:** Auto-organizacao, emergencia, resiliencia

5. **🔄 Sequencial vs Paralelo na pratica**
   - **O que e:** Comparacao direta com exemplos — OpenCode Swarm (sequencial) vs oh-my-openagent (paralelo)
   - **Por que aprender:** Saber escolher a arquitetura certa para cada projeto
   - **Conceitos-chave:** Trade-offs, race conditions, consistencia vs velocidade

6. **🎨 Hibrido: o melhor dos dois mundos**
   - **O que e:** Combinar sequencial para planejamento e paralelo para execucao
   - **Por que aprender:** A maioria dos sistemas reais usa abordagem hibrida
   - **Conceitos-chave:** Plan sequencial → Execute paralelo, gates de qualidade

### Recursos:
- [Swarm Architectures - docs.swarms.world](https://docs.swarms.world/en/latest/swarms/concept/swarm_architectures/)
- [Top 5 AI Agent Architectures 2025 - MarkTechPost](https://www.marktechpost.com/2025/11/15/comparing-the-top-5-ai-agent-architectures-in-2025-hierarchical-swarm-meta-learning-modular-evolutionary/)

---

## Modulo 1.4 - Papeis e Especializacao de Agentes

**Duracao:** ~40 min | **Nivel:** Iniciante

### Topicos:

1. **👔 O Orquestrador: cerebro do swarm**
   - **O que e:** Agente central que recebe tarefas, cria planos e delega — nao para ate terminar
   - **Por que aprender:** Sem bom orquestrador, o swarm e caos
   - **Conceitos-chave:** Sisyphus (OMO), Architect (opencode-swarm), Supervisor

2. **📐 O Planejador: antes de executar**
   - **O que e:** Faz entrevista, identifica escopo, constroi plano detalhado
   - **Por que aprender:** Planejamento ruim = execucao ruim
   - **Conceitos-chave:** Prometheus (OMO), discovery questions, spec files

3. **💻 O Executor: mao na massa**
   - **O que e:** Agente que escreve codigo, implementa solucoes concretas
   - **Por que aprender:** E onde o trabalho real acontece
   - **Conceitos-chave:** Hephaestus (OMO), Coder (opencode-swarm), tarefas atomicas

4. **🔍 O Revisor: olhar critico**
   - **O que e:** Avalia corretude, seguranca e qualidade do que foi produzido
   - **Por que aprender:** Revisao automatica reduz bugs drasticamente
   - **Conceitos-chave:** Reviewer, Critic, modelo diferente do executor (anti-blindspot)

5. **🧪 O Testador: prova que funciona**
   - **O que e:** Gera testes de verificacao e adversariais
   - **Por que aprender:** Codigo sem teste e codigo com bug escondido
   - **Conceitos-chave:** Test Engineer, testes unitarios, testes adversariais

6. **🔎 Agentes de suporte: explorador, pesquisador, visual**
   - **O que e:** Explorer (escaneia codebase), Librarian (busca docs), Multimodal Looker (analisa imagens)
   - **Por que aprender:** Agentes auxiliares fornecem contexto que melhora todo o swarm
   - **Conceitos-chave:** Read-only, pesquisa, contexto tecnico, analise visual

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 1.5 - Comunicacao entre Agentes

**Duracao:** ~35 min | **Nivel:** Intermediario

### Topicos:

1. **📡 Por que comunicacao importa**
   - **O que e:** Agentes precisam trocar informacao para coordenar trabalho sem conflitos
   - **Por que aprender:** Comunicacao ruim = agentes que se atrapalham ou duplicam trabalho
   - **Conceitos-chave:** Coordenacao, sincronizacao, evitar conflitos

2. **🔄 Handoffs: passando o bastao**
   - **O que e:** Um agente completa sua tarefa e transfere controle para o proximo
   - **Por que aprender:** Padrao mais simples e eficaz para pipelines
   - **Conceitos-chave:** Transfer, context variables, OpenAI Swarm

3. **📋 Estado compartilhado**
   - **O que e:** Agentes leem e escrevem em um estado global (context, plano, evidencias)
   - **Por que aprender:** Essencial para swarms paralelos que precisam de coordenacao
   - **Conceitos-chave:** State machine, .swarm/ directory, plan.md

4. **🔒 Zonas seguras: evitar interferencia**
   - **O que e:** Cada agente trabalha em arquivos/areas distintos para evitar conflitos
   - **Por que aprender:** Conflitos de merge entre agentes destroem produtividade
   - **Conceitos-chave:** File locking, zonas exclusivas, hash unico por linha

5. **📨 Protocolos emergentes: MCP, A2A, ACP**
   - **O que e:** MCP (ferramentas), A2A (agente-para-agente), ACP (dialogo estruturado)
   - **Por que aprender:** Sao os padroes que a industria esta adotando em 2026
   - **Conceitos-chave:** Anthropic MCP, Google A2A, IBM ACP, interoperabilidade

6. **📊 Feedback e auto-correcao**
   - **O que e:** Orquestrador recebe resultado, avalia, pede correcoes se necessario
   - **Por que aprender:** Auto-correcao e o que torna swarms realmente autonomos
   - **Conceitos-chave:** Loop de feedback, maker-checker, quality gates

### Recursos:
- [MCP vs A2A - Auth0](https://auth0.com/blog/mcp-vs-a2a/)
- [Survey of Agent Interoperability Protocols - arXiv](https://arxiv.org/html/2505.02279v1)

---

## Modulo 1.6 - Modelos e Custos: estrategia inteligente

**Duracao:** ~35 min | **Nivel:** Iniciante

### Topicos:

1. **🧩 Modelo certo para cada papel**
   - **O que e:** Usar modelos potentes (Opus, GPT-5.3) para orquestrador e modelos leves para tarefas simples
   - **Por que aprender:** Otimizar custo sem sacrificar qualidade
   - **Conceitos-chave:** Modelo potente para raciocinio, modelo leve para execucao

2. **🔀 Modelos heterogeneos (anti-blindspot)**
   - **O que e:** Coder e Reviewer usam modelos de providers diferentes deliberadamente
   - **Por que aprender:** Modelos diferentes capturam erros que um unico ignoraria
   - **Conceitos-chave:** Cross-provider, dados de treino distintos, complementaridade

3. **💰 Modelos gratuitos: quando usar**
   - **O que e:** OpenCode oferece modelos gratuitos (Big Pickle, minimax) para tarefas de baixo valor
   - **Por que aprender:** Reduzir custos drasticamente sem impacto na qualidade final
   - **Conceitos-chave:** OpenCode Zen, modelos gratuitos, custo zero para exploracao

4. **📈 Estrategia de custo por agente**
   - **O que e:** Claude Opus para Sisyphus/Prometheus, Codex 5.3 para Hephaestus, gratuitos para Explore/Librarian
   - **Por que aprender:** Aplicar na pratica a otimizacao de custos
   - **Conceitos-chave:** Tier de modelos, mapeamento agente→modelo

5. **⚡ Limites e rate limits**
   - **O que e:** Cada provider tem limites de uso — saber contornar sem interromper o swarm
   - **Por que aprender:** Swarms consomem tokens rapido — planejamento evita interrupcoes
   - **Conceitos-chave:** Tokens por minuto, fallback, provider switching

6. **🏢 OpenCode como hub multi-modelo**
   - **O que e:** OpenCode permite combinar Anthropic, OpenAI, Google, modelos gratuitos no mesmo fluxo
   - **Por que aprender:** Flexibilidade maxima sem lock-in de ecossistema
   - **Conceitos-chave:** Provider agnostico, multi-ecosystem, configuracao por agente

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 1.7 - Sequencial vs Paralelo: estudo comparativo

**Duracao:** ~40 min | **Nivel:** Intermediario

### Topicos:

1. **📐 OpenCode Swarm: o modelo sequencial**
   - **O que e:** Pipeline de 8 subagentes em serie — Explorer → SME → Architect → Critic → Coder → Reviewer → Test → Docs
   - **Por que aprender:** Entender a abordagem serial disciplinada e seus beneficios
   - **Conceitos-chave:** Gated pipeline, state machine, sem race conditions

2. **⚡ oh-my-openagent: o modelo paralelo**
   - **O que e:** Sisyphus coordena multiplos agentes trabalhando simultaneamente em tarefas diferentes
   - **Por que aprender:** Entender como paralelismo real funciona na pratica
   - **Conceitos-chave:** Background agents, zonas seguras, merge de resultados

3. **📊 Benchmarks: velocidade vs confiabilidade**
   - **O que e:** Sequencial e mais lento mas mais confiavel; paralelo e rapido mas requer coordenacao
   - **Por que aprender:** Dados concretos para tomar decisoes informadas
   - **Conceitos-chave:** Taxa de sucesso 6% → 68.3% (com hash checking), trade-offs

4. **🔍 18 decisoes de design do opencode-swarm**
   - **O que e:** Documento design-rationale.md com justificativas para cada escolha arquitetural
   - **Por que aprender:** Aprender com decisoes reais e bem documentadas
   - **Conceitos-chave:** Serial over parallel, persistent memory, heterogeneous models

5. **🎯 Gates de qualidade automatizados**
   - **O que e:** 6 gates por tarefa: syntax, placeholder, SAST, SBOM, build, quality budget
   - **Por que aprender:** Qualidade automatizada e essencial em qualquer swarm de producao
   - **Conceitos-chave:** Tree-sitter, OWASP Top 10, dependency tracking

6. **🔄 Sistema Curator: drift plano vs realidade**
   - **O que e:** Monitoramento quantitativo do desvio entre plano original e implementacao real
   - **Por que aprender:** Conceito avancado e unico — medir drift e corrigir rota
   - **Conceitos-chave:** Drift score 0.0-1.0, ALIGNED/MINOR/MAJOR/OFF_SPEC

### Recursos:
- [GitHub - zaxbysauce/opencode-swarm](https://github.com/zaxbysauce/opencode-swarm)

---

## Modulo 1.8 - Mapa do ecossistema agentico

**Duracao:** ~30 min | **Nivel:** Iniciante

### Topicos:

1. **🗺️ Frameworks principais: CrewAI, LangGraph, AutoGen**
   - **O que e:** Os tres frameworks mais populares para construir swarms
   - **Por que aprender:** Saber o que existe antes de escolher
   - **Conceitos-chave:** Role-based (CrewAI), graph-based (LangGraph), conversational (AutoGen)

2. **🔧 Ferramentas praticas: OpenCode, Claude Code, Codex**
   - **O que e:** Ambientes de desenvolvimento com suporte nativo a multiagentes
   - **Por que aprender:** Comecar a usar swarms sem construir do zero
   - **Conceitos-chave:** Plugins, configuracao, pratica imediata

3. **📡 Protocolos: MCP, A2A, ACP**
   - **O que e:** Padroes de comunicacao entre agentes e ferramentas
   - **Por que aprender:** Interoperabilidade e o futuro — evitar lock-in
   - **Conceitos-chave:** Anthropic MCP, Google A2A (Linux Foundation), IBM ACP

4. **🏪 Plugins e extensoes: oh-my-openagent, Superpowers**
   - **O que e:** Plugins que transformam ferramentas existentes em sistemas multiagentes
   - **Por que aprender:** Atalho para comecar sem construir do zero
   - **Conceitos-chave:** OMO (41k stars), Superpowers (27k stars)

5. **📚 Cursos e referencias essenciais**
   - **O que e:** Melhores recursos para aprofundar: DeepLearning.AI, LangChain Academy, Zero To Mastery
   - **Por que aprender:** Roadmap de aprendizado continuo
   - **Conceitos-chave:** Andrew Ng (Agentic AI), LangGraph Academy, CrewAI Learn

6. **⚠️ Alerta: a armadilha multiagente**
   - **O que e:** Gartner projeta 40%+ dos projetos agenticos cancelados ate 2027 por custos escalantes
   - **Por que aprender:** Evitar erros comuns — excesso de especializacao, falta de governanca
   - **Conceitos-chave:** The Multi-Agent Trap, cognition governance, custo vs valor

### Recursos:
- [CrewAI vs LangGraph vs AutoGen - DataCamp](https://www.datacamp.com/tutorial/crewai-vs-langgraph-vs-autogen)
- [The Multi-Agent Trap - Towards Data Science](https://towardsdatascience.com/the-multi-agent-trap/)
- Curso DeepLearning.AI: [Agentic AI (Andrew Ng)](https://www.deeplearning.ai/courses/agentic-ai/)

---

# TRILHA 2: TECNICAS (Blue)

> **Aprenda a construir e configurar swarms com ferramentas reais**
>
> **Ilustracao principal:** `doc/photo_5035387927072017301_w.jpg` (diagrama arquitetural completo)

## Modulo 2.1 - OpenAI Swarm: seu primeiro swarm

**Duracao:** ~40 min | **Nivel:** Iniciante

### Topicos:

1. **🎓 OpenAI Swarm: ferramenta educacional**
   - **O que e:** Framework minimalista e experimental da OpenAI para aprender principios de swarms
   - **Por que aprender:** Codigo limpo e legivel — melhor ponto de entrada para entender a mecanica
   - **Conceitos-chave:** Educacional, nao para producao, principios fundamentais

2. **🤖 Conceito de Agent no Swarm**
   - **O que e:** Agente = conjunto de instrucoes + funcoes + modelo — simples assim
   - **Por que aprender:** Entender a unidade basica antes de sistemas complexos
   - **Conceitos-chave:** Instructions, functions, model, name

3. **🔄 Handoffs: transferencia de controle**
   - **O que e:** Um agente decide passar o controle para outro agente especializado
   - **Por que aprender:** Handoff e o mecanismo central de orquestracao no Swarm
   - **Conceitos-chave:** transfer_to_agent(), context variables, routing

4. **📦 Context Variables: estado compartilhado**
   - **O que e:** Dicionario de variaveis acessivel por todos os agentes do swarm
   - **Por que aprender:** E como agentes compartilham informacao sem acoplamento
   - **Conceitos-chave:** context_variables, passagem por referencia

5. **💻 Exemplo pratico: atendimento ao cliente**
   - **O que e:** Swarm com agente de triagem → vendas → suporte tecnico → reembolso
   - **Por que aprender:** Caso de uso classico que demonstra todos os conceitos
   - **Conceitos-chave:** Triage agent, specialist agents, routing logic

6. **🔀 De Swarm para producao: proximos passos**
   - **O que e:** Como migrar conceitos do Swarm educacional para frameworks de producao
   - **Por que aprender:** Transicao natural para CrewAI/LangGraph
   - **Conceitos-chave:** Limitacoes, alternativas, evolucao

### Recursos:
- [GitHub - openai/swarm](https://github.com/openai/swarm)

---

## Modulo 2.2 - CrewAI: equipes de agentes

**Duracao:** ~45 min | **Nivel:** Intermediario

### Topicos:

1. **👥 CrewAI: o mais popular**
   - **O que e:** Framework role-based que organiza agentes como uma equipe com cargos e responsabilidades
   - **Por que aprender:** Maior comunidade (100k+ devs certificados), 1.1 bilhao de tarefas orquestradas
   - **Conceitos-chave:** Agents, Tasks, Crews, Flows

2. **🎭 Definindo agentes com papeis**
   - **O que e:** Cada agente tem role, goal, backstory — como um funcionario com cargo definido
   - **Por que aprender:** Modelo mental intuitivo para qualquer equipe
   - **Conceitos-chave:** Role, goal, backstory, tools, llm

3. **📋 Tasks e delegacao**
   - **O que e:** Tarefas com descricao, agente responsavel e criterio de conclusao
   - **Por que aprender:** Tarefas bem definidas = execucao previsivel
   - **Conceitos-chave:** Description, agent, expected_output, context

4. **🔧 Tools e integracao**
   - **O que e:** Ferramentas que agentes podem usar: busca web, leitura de arquivos, APIs
   - **Por que aprender:** Agentes sem ferramentas sao limitados
   - **Conceitos-chave:** CrewAI Tools, custom tools, MCP servers

5. **🔄 Flows: orquestracao avancada**
   - **O que e:** Workflows complexos com condicoes, loops e ramificacoes
   - **Por que aprender:** Projetos reais precisam de logica de negocio alem de delegacao simples
   - **Conceitos-chave:** Flow, Router, conditional execution

6. **📦 Guardrails e memoria**
   - **O que e:** Limites de seguranca e memoria persistente entre execucoes
   - **Por que aprender:** Producao exige controle e continuidade
   - **Conceitos-chave:** Input/output guardrails, short/long-term memory

### Recursos:
- [docs.crewai.com](https://docs.crewai.com)
- [Curso DeepLearning.AI - Multi AI Agent Systems with crewAI](https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/)
- [GitHub - crewAIInc/crewAI-examples](https://github.com/crewAIInc/crewAI-examples)

---

## Modulo 2.3 - LangGraph: controle total com grafos

**Duracao:** ~45 min | **Nivel:** Intermediario

### Topicos:

1. **📊 LangGraph: workflows como grafos**
   - **O que e:** Framework graph-based da LangChain onde estados fluem por nos e arestas
   - **Por que aprender:** Maximo controle sobre fluxo — ideal para workflows complexos
   - **Conceitos-chave:** StateGraph, Nodes, Edges, Checkpointing

2. **🔲 Nos: unidades de processamento**
   - **O que e:** Funcoes que recebem estado, processam e retornam estado atualizado
   - **Por que aprender:** Cada no pode ser um agente, ferramenta ou logica de negocio
   - **Conceitos-chave:** Node functions, state transformation

3. **➡️ Arestas: fluxo de controle**
   - **O que e:** Conexoes entre nos — podem ser condicionais (if/else) ou fixas
   - **Por que aprender:** E onde a logica de roteamento vive
   - **Conceitos-chave:** Conditional edges, routing, bifurcacao

4. **💾 Checkpointing: execucao duravel**
   - **O que e:** Salvar estado a cada passo para retomar apos falhas
   - **Por que aprender:** Essencial para swarms de longa duracao em producao
   - **Conceitos-chave:** State persistence, recovery, durability

5. **👤 Human-in-the-loop**
   - **O que e:** Inserir pontos de aprovacao humana no fluxo do grafo
   - **Por que aprender:** Governanca e compliance exigem verificacao humana
   - **Conceitos-chave:** Interrupt, resume, approval gates

6. **🏗️ Supervisors e subgraphs**
   - **O que e:** Grafos dentro de grafos — supervisor no topo coordenando subgrafos especializados
   - **Por que aprender:** Composicao e a forma de escalar complexidade
   - **Conceitos-chave:** Subgraph, supervisor pattern, hierarquia

### Recursos:
- [docs.langchain.com/oss/python/langgraph](https://docs.langchain.com/oss/python/langgraph/overview)
- [LangChain Academy - Introduction to LangGraph](https://academy.langchain.com/courses/intro-to-langgraph) (gratuito)
- [GitHub - langchain-ai/langgraph](https://github.com/langchain-ai/langgraph)

---

## Modulo 2.4 - oh-my-openagent na pratica

**Duracao:** ~50 min | **Nivel:** Intermediario

### Topicos:

1. **🔌 Instalacao e configuracao**
   - **O que e:** Instalar Bun, OMO e configurar para Claude, OpenAI, Gemini ou modelos gratuitos
   - **Por que aprender:** Setup pratico para comecar a usar swarms hoje
   - **Conceitos-chave:** bunx, opencode.json, global vs por projeto

2. **⚡ Modo ultrawork: velocidade maxima**
   - **O que e:** Escrever `ultrawork` e deixar o swarm executar ate terminar
   - **Por que aprender:** Para quando voce sabe exatamente o que quer
   - **Conceitos-chave:** Execucao continua, sem intervencao, todos agentes ativados

3. **📋 Modo Prometheus: entrevista + plano**
   - **O que e:** Agente planificador faz entrevista detalhada antes de comecar a executar
   - **Por que aprender:** Melhor abordagem para projetos novos — contexto completo
   - **Conceitos-chave:** Tab para Prometheus, entrevista, /start-work

4. **🎯 Categorias de roteamento do Sisyphus**
   - **O que e:** Visual Engineering, Deep Research, Quick Changes, UltraBrain — roteamento automatico
   - **Por que aprender:** Entender como o orquestrador decide qual agente usar
   - **Conceitos-chave:** Categoria automatica, tipo de tarefa, modelo otimizado

5. **⚙️ Configurando modelos por agente**
   - **O que e:** Arquivo `.opencode/oh-my-opencode.jsonc` para definir modelo de cada agente
   - **Por que aprender:** Otimizar custo e desempenho personalizando modelos
   - **Conceitos-chave:** sisyphus→opus, hephaestus→codex, explore→gratuito

6. **🏗️ Projeto completo: landing page do zero**
   - **O que e:** Demonstracao end-to-end: entrevista → plano → execucao paralela → revisao → resultado
   - **Por que aprender:** Ver o swarm em acao em um caso real
   - **Conceitos-chave:** Workflow completo, auto-correcao, resultado funcional

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 2.5 - AutoGen e Microsoft Agent Framework

**Duracao:** ~40 min | **Nivel:** Intermediario

### Topicos:

1. **💬 AutoGen: agentes conversacionais**
   - **O que e:** Framework da Microsoft onde agentes interagem como dialogos entre si
   - **Por que aprender:** Abordagem unica — conversacao como mecanismo de coordenacao
   - **Conceitos-chave:** ConversableAgent, GroupChat, colaboracao conversacional

2. **🔄 Evolucao: Microsoft Agent Framework**
   - **O que e:** AutoGen + Semantic Kernel combinados no novo framework enterprise da Microsoft
   - **Por que aprender:** E para onde o AutoGen esta migrando — importante saber
   - **Conceitos-chave:** State management, type safety, middleware, telemetria

3. **💻 Coding agents com Docker**
   - **O que e:** AutoGen executa codigo em containers Docker isolados — seguranca maxima
   - **Por que aprender:** Padrao ouro para agentes que geram e executam codigo
   - **Conceitos-chave:** Docker executor, sandboxing, code generation + execution

4. **🗣️ GroupChat: conversacao multiagente**
   - **O que e:** Multiplos agentes conversam em grupo com manager que controla turnos
   - **Por que aprender:** Padrao unico do AutoGen — debate e refinamento entre agentes
   - **Conceitos-chave:** GroupChatManager, turn management, consensus

5. **🔧 Tools e Function Calling**
   - **O que e:** Agentes podem chamar funcoes externas durante a conversacao
   - **Por que aprender:** Estender capacidades dos agentes conversacionais
   - **Conceitos-chave:** register_function, tool_use, return values

6. **📊 Quando usar AutoGen vs CrewAI vs LangGraph**
   - **O que e:** Comparacao pratica: conversacional (AutoGen) vs role-based (CrewAI) vs graph (LangGraph)
   - **Por que aprender:** Escolher o framework certo economiza semanas de trabalho
   - **Conceitos-chave:** Tabela comparativa, criterios de escolha, casos de uso ideais

### Recursos:
- [microsoft.github.io/autogen](https://microsoft.github.io/autogen/stable/)
- [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/)
- [GitHub - microsoft/autogen](https://github.com/microsoft/autogen)

---

## Modulo 2.6 - Protocolos de comunicacao: MCP, A2A, ACP

**Duracao:** ~40 min | **Nivel:** Intermediario-Avancado

### Topicos:

1. **🔌 MCP: Model Context Protocol**
   - **O que e:** Protocolo da Anthropic que padroniza como agentes acessam ferramentas e dados externos
   - **Por que aprender:** Elimina APIs customizadas — padrao universal para ferramentas
   - **Conceitos-chave:** Tools, data sources, resources, prompts, sampling

2. **🤝 A2A: Agent-to-Agent Protocol**
   - **O que e:** Protocolo do Google (agora Linux Foundation) para comunicacao direta entre agentes
   - **Por que aprender:** E o padrao emergente mais importante para interoperabilidade
   - **Conceitos-chave:** Agent Cards, task management, streaming, sem lock-in

3. **💬 ACP: Agent Communication Protocol**
   - **O que e:** Protocolo da IBM para dialogo estruturado entre agentes heterogeneos
   - **Por que aprender:** Enfase em intencao e semantica — ideal para enterprise
   - **Conceitos-chave:** Intent, structured dialogue, semantic communication

4. **📊 MCP vs A2A: quando usar cada um**
   - **O que e:** MCP para conectar agente→ferramenta; A2A para conectar agente→agente
   - **Por que aprender:** Sao complementares, nao concorrentes
   - **Conceitos-chave:** MCP = vertical (dados), A2A = horizontal (colaboracao)

5. **🔧 Configurando MCP na pratica**
   - **O que e:** Setup de MCP servers para conectar agentes a APIs, bancos de dados, servicos
   - **Por que aprender:** Hands-on com o protocolo mais adotado
   - **Conceitos-chave:** claude_desktop_config.json, servers, stdio/sse

6. **🔮 Futuro: interoperabilidade universal**
   - **O que e:** Cenario onde agentes de diferentes providers colaboram via protocolos abertos
   - **Por que aprender:** Preparar-se para o futuro multi-vendor
   - **Conceitos-chave:** Open standards, federation, trust

### Recursos:
- [A2A Protocol - DeepLearning.AI](https://www.deeplearning.ai/short-courses/a2a-the-agent2agent-protocol/)
- [MCP, ACP, A2A Explained - Boomi](https://boomi.com/blog/what-is-mcp-acp-a2a/)
- [A2A Protocol Official](https://a2a-protocol.org/latest/)

---

## Modulo 2.7 - Padroes de orquestracao

**Duracao:** ~40 min | **Nivel:** Avancado

### Topicos:

1. **🎯 Supervisor Pattern**
   - **O que e:** Agente central roteia tarefas e sintetiza resultados — padrao mais usado
   - **Por que aprender:** E o "default" para a maioria dos projetos
   - **Conceitos-chave:** Central routing, result synthesis, governanca

2. **✅ Maker-Checker Pattern**
   - **O que e:** Um agente executa, outro verifica — ideal para alta acuracia
   - **Por que aprender:** Reduz erros drasticamente em tarefas criticas
   - **Conceitos-chave:** Gerador + Verificador, dual review, cross-model

3. **🔀 Adaptive Agent Network**
   - **O que e:** Agentes se auto-organizam dinamicamente baseado na tarefa
   - **Por que aprender:** Flexibilidade maxima para cenarios imprevisiveis
   - **Conceitos-chave:** Auto-routing, capability matching, emergencia

4. **🔗 Mediator Pattern**
   - **O que e:** Agente intermediario resolve conflitos entre agentes especializados
   - **Por que aprender:** Essencial quando agentes discordam ou geram resultados conflitantes
   - **Conceitos-chave:** Conflict resolution, consensus, arbitration

5. **📦 Regra das tres balas (opencode-swarm)**
   - **O que e:** Se nao cabe em TASK + FILE + CONSTRAINT em tres bullets, a tarefa e grande demais
   - **Por que aprender:** Heuristica pratica para dimensionar tarefas de agentes
   - **Conceitos-chave:** Atomicidade, max 2 arquivos por tarefa, decomposicao

6. **🏗️ Supervisores de supervisores**
   - **O que e:** Hierarquia multinivel — supervisor principal coordena supervisores de area
   - **Por que aprender:** Escalar para projetos muito grandes
   - **Conceitos-chave:** Hierarchical MAS, meta-orchestration, delegation chains

### Recursos:
- [Choosing the Right Orchestration Pattern - Kore.ai](https://www.kore.ai/blog/choosing-the-right-orchestration-pattern-for-multi-agent-systems/)
- [Designing Effective Multi-Agent Architectures - O'Reilly](https://www.oreilly.com/radar/designing-effective-multi-agent-architectures/)

---

## Modulo 2.8 - Swarms Framework e outros

**Duracao:** ~35 min | **Nivel:** Intermediario

### Topicos:

1. **🐝 Swarms Framework (Kye Gomez)**
   - **O que e:** Framework enterprise-grade focado em producao — diferente do OpenAI Swarm educacional
   - **Por que aprender:** Opcao madura para deploy em escala
   - **Conceitos-chave:** Production-ready, multiple swarm types, enterprise

2. **🏢 Agency Swarm (VRSEN)**
   - **O que e:** Orquestracao confiavel com estrutura de agencia — agentes como departamentos
   - **Por que aprender:** Modelo organizacional intuitivo
   - **Conceitos-chave:** Agency structure, reliable orchestration

3. **🐙 Camel-AI e debate multiagente**
   - **O que e:** Framework focado em comunicacao entre agentes atraves de debate
   - **Por que aprender:** Abordagem unica — consenso por argumentacao
   - **Conceitos-chave:** Role-playing, debate, consensus building

4. **🔧 Claude Code Agent SDK**
   - **O que e:** SDK da Anthropic para construir agentes customizados com Claude
   - **Por que aprender:** Integracao nativa com o melhor modelo para raciocinio
   - **Conceitos-chave:** Agent SDK, tool_use, streaming, subagentes

5. **📊 Tabela comparativa completa**
   - **O que e:** Comparacao lado a lado de todos os frameworks cobertos
   - **Por que aprender:** Referencia rapida para decisoes
   - **Conceitos-chave:** Stars, paradigma, linguagem, complexidade, caso ideal

6. **🎯 Escolhendo o framework certo**
   - **O que e:** Arvore de decisao: iniciante? → OpenAI Swarm. Equipe? → CrewAI. Controle? → LangGraph. Enterprise? → Swarms
   - **Por que aprender:** Atalho para a decisao mais importante do projeto
   - **Conceitos-chave:** Decision tree, criterios, trade-offs

### Recursos:
- [docs.swarms.world](https://docs.swarms.world/en/latest/)
- [GitHub - VRSEN/agency-swarm](https://github.com/VRSEN/agency-swarm)
- [Best AI Agent Frameworks 2025 - Maxim AI](https://www.getmaxim.ai/articles/top-5-ai-agent-frameworks-in-2025-a-practical-guide-for-ai-builders/)

---

# TRILHA 3: PRATICA AVANCADA (Purple)

> **Construa, otimize e coloque swarms em producao**
>
> **Ilustracao principal:** `doc/ChatGPT Image 19...06_04_43.png` (exercito de agentes cyberpunk)

## Modulo 3.1 - Projeto 1: sistema de atendimento multiagente

**Duracao:** ~60 min | **Nivel:** Intermediario

### Topicos:

1. **🎯 Definindo o projeto: atendimento ao cliente**
   - **O que e:** Swarm com triagem automatica → agentes especialistas (vendas, suporte, billing)
   - **Por que aprender:** Caso de uso real mais comum para swarms em producao
   - **Conceitos-chave:** Customer service, routing, especialistas

2. **🤖 Agente de triagem: roteamento inteligente**
   - **O que e:** Primeiro agente classifica a intencao e direciona ao especialista correto
   - **Por que aprender:** E o componente mais critico do sistema
   - **Conceitos-chave:** Intent classification, routing rules, fallback

3. **👥 Agentes especialistas: implementacao**
   - **O que e:** Cada especialista com instrucoes, ferramentas e tom de voz especificos
   - **Por que aprender:** Especializacao e o que torna o swarm eficaz
   - **Conceitos-chave:** Domain expertise, tool access, personality

4. **🔄 Handoffs e escalacao**
   - **O que e:** Transferencia de contexto entre agentes e escalacao para humano quando necessario
   - **Por que aprender:** Transicoes suaves sao essenciais para experiencia do usuario
   - **Conceitos-chave:** Context passing, escalation rules, human-in-the-loop

5. **💾 Memoria de conversa**
   - **O que e:** Manter historico entre agentes e entre sessoes do mesmo cliente
   - **Por que aprender:** Cliente nao deve repetir informacao a cada troca de agente
   - **Conceitos-chave:** Conversation memory, session state, customer profile

6. **📊 Metricas e monitoramento**
   - **O que e:** Tracking de resolucao, tempo, satisfacao, uso de tokens
   - **Por que aprender:** Sem metricas, impossivel otimizar
   - **Conceitos-chave:** Resolution rate, CSAT, token cost, latency

### Recursos:
- Exemplo: OpenAI Swarm airline/customer_service
- [CrewAI Examples - Customer Support](https://github.com/crewAIInc/crewAI-examples)

---

## Modulo 3.2 - Projeto 2: equipe de desenvolvimento autonoma

**Duracao:** ~60 min | **Nivel:** Avancado

### Topicos:

1. **🏗️ Arquitetura: replicando oh-my-openagent**
   - **O que e:** Construir um swarm de desenvolvimento com orquestrador, planejador, coder, revisor e testador
   - **Por que aprender:** Entender internamente como OMO funciona
   - **Conceitos-chave:** Sisyphus-like orchestrator, specialized agents

2. **📋 Fase de planejamento: entrevista e spec**
   - **O que e:** Agente planificador faz discovery questions e gera spec detalhada
   - **Por que aprender:** Plano bem feito = execucao sem retrabalho
   - **Conceitos-chave:** Discovery, requirements, spec.md, acceptance criteria

3. **💻 Fase de execucao: coding com zonas seguras**
   - **O que e:** Multiplos agentes codificam em paralelo sem conflitos
   - **Por que aprender:** Paralelismo real requer coordenacao cuidadosa
   - **Conceitos-chave:** File ownership, atomic tasks, merge strategy

4. **🔍 Fase de revisao: cross-model review**
   - **O que e:** Agente de revisao usa modelo diferente do coder para detectar blindspots
   - **Por que aprender:** Anti-blindspot e tecnica comprovada de qualidade
   - **Conceitos-chave:** Different provider, review checklist, APPROVED/NEEDS_REVISION

5. **🧪 Fase de teste: testes automatizados**
   - **O que e:** Agente testador gera e executa testes automaticamente
   - **Por que aprender:** Garantir que o codigo funciona antes de entregar
   - **Conceitos-chave:** Unit tests, integration tests, adversarial tests

6. **📝 Fase de documentacao: docs automaticos**
   - **O que e:** Agente documentador registra decisoes, mudancas e API
   - **Por que aprender:** Documentacao e o que permite manter o projeto vivo
   - **Conceitos-chave:** Auto-docs, changelog, decision log

### Recursos:
- [GitHub - zaxbysauce/opencode-swarm](https://github.com/zaxbysauce/opencode-swarm) (architecture.md, design-rationale.md)

---

## Modulo 3.3 - Memoria e persistencia em swarms

**Duracao:** ~45 min | **Nivel:** Avancado

### Topicos:

1. **💾 O problema: LLMs sao stateless**
   - **O que e:** Sem memoria, cada interacao comeca do zero — impossivel para projetos longos
   - **Por que aprender:** Memoria e o que diferencia um swarm util de um demo
   - **Conceitos-chave:** Context window limit, information loss, session boundary

2. **📁 Memoria em disco: padrao .swarm/**
   - **O que e:** Diretorio persistente com plan.md, context.md, evidence/, history/
   - **Por que aprender:** Abordagem pratica do opencode-swarm — funciona sem infraestrutura extra
   - **Conceitos-chave:** File-based memory, plan.json, Zod validation

3. **⚡ Memoria efemera: Redis para estado de execucao**
   - **O que e:** Cache em memoria para dados durante a execucao do swarm
   - **Por que aprender:** Performance em tempo real sem overhead de disco
   - **Conceitos-chave:** Redis, session state, TTL, eviction

4. **🧠 Memoria de longo prazo: Vector DB**
   - **O que e:** Conhecimento persistente que sobrevive entre sessoes (embeddings + similaridade)
   - **Por que aprender:** Agentes que lembram e aprendem ao longo do tempo
   - **Conceitos-chave:** Vector store, embeddings, semantic search, ChromaDB, Pinecone

5. **📊 Decision Trace: rastreabilidade**
   - **O que e:** Logs estruturados de cada decisao: prompt, resposta, resultado, avaliacao
   - **Por que aprender:** Auditoria, debugging e reproducibilidade
   - **Conceitos-chave:** Decision log, evidence collection, reproducibility

6. **🔄 Progressao: RAG → Agentic RAG → Agent Memory**
   - **O que e:** Evolucao de busca simples para agentes que decidem o que lembrar e esquecer
   - **Por que aprender:** Entender o roadmap de evolucao de memoria
   - **Conceitos-chave:** RAG basico, Agentic RAG, episodic memory, memory curation

### Recursos:
- [opencode-swarm design-rationale.md](https://github.com/zaxbysauce/opencode-swarm) (decision 3: persistent memory)
- [What is Agentic RAG? - IBM](https://www.ibm.com/think/topics/agentic-rag)

---

## Modulo 3.4 - Qualidade e seguranca em swarms

**Duracao:** ~45 min | **Nivel:** Avancado

### Topicos:

1. **🔒 Gates de qualidade automatizados**
   - **O que e:** Verificacoes automaticas a cada tarefa: syntax, placeholders, SAST, SBOM, build, quality
   - **Por que aprender:** Qualidade sistematica — nao depende de revisao humana
   - **Conceitos-chave:** 6 gates, Tree-sitter (9+ linguagens), pre_check_batch

2. **🛡️ SAST: analise de seguranca estatica**
   - **O que e:** Detectar vulnerabilidades OWASP Top 10 automaticamente antes do deploy
   - **Por que aprender:** Codigo gerado por IA frequentemente tem vulnerabilidades
   - **Conceitos-chave:** Injection, XSS, SSRF, path traversal, hardcoded secrets

3. **📦 SBOM: rastreamento de dependencias**
   - **O que e:** Software Bill of Materials — inventario de todas as dependencias e suas vulnerabilidades
   - **Por que aprender:** Supply chain attacks sao a maior ameaca de 2026
   - **Conceitos-chave:** Dependency tracking, CVE checking, license compliance

4. **🧹 Anti-slop: detectando codigo lixo**
   - **O que e:** Auditoria de padroes ruins em codigo gerado por IA: duplicacao, God Functions, testing theater
   - **Por que aprender:** IA gera codigo "bonito" que esconde problemas graves
   - **Conceitos-chave:** AI Slop Review, 268 assertions testando texto de prompt (anti-pattern real)

5. **🔍 Placeholder scan: nada fica incompleto**
   - **O que e:** Detectar TODOs, stubs, funcoes vazias antes de declarar tarefa completa
   - **Por que aprender:** Agentes frequentemente deixam placeholders que parecem codigo real
   - **Conceitos-chave:** TODO detection, stub identification, completeness check

6. **📊 Quality budget: metricas de manutenibilidade**
   - **O que e:** Limites numericos para complexidade, tamanho de funcao, acoplamento
   - **Por que aprender:** Manter codigo mantivel a longo prazo
   - **Conceitos-chave:** Cyclomatic complexity, function length, coupling metrics

### Recursos:
- [opencode-swarm AI_SLOP_REVIEW.md](https://github.com/zaxbysauce/opencode-swarm)
- [opencode-swarm architecture.md](https://github.com/zaxbysauce/opencode-swarm) (QA Gates section)

---

## Modulo 3.5 - Projeto 3: pesquisa profunda multiagente

**Duracao:** ~50 min | **Nivel:** Avancado

### Topicos:

1. **🔬 Deep Research: o que e**
   - **O que e:** Sistema onde multiplos agentes pesquisam, sintetizam e produzem relatorio abrangente
   - **Por que aprender:** Um dos usos mais poderosos de swarms — substitui horas de pesquisa manual
   - **Conceitos-chave:** Multi-source research, synthesis, structured output

2. **🔎 Agentes de busca: web, docs, github**
   - **O que e:** Agentes especializados em fontes diferentes trabalhando em paralelo
   - **Por que aprender:** Cobertura ampla + velocidade = pesquisa superior
   - **Conceitos-chave:** Web search, documentation crawling, GitHub code search

3. **📊 Agente sintetizador: reunir e filtrar**
   - **O que e:** Agente que consolida resultados, remove duplicatas e organiza hierarquicamente
   - **Por que aprender:** Dados brutos sem sintese sao inuteis
   - **Conceitos-chave:** Deduplication, ranking, structured synthesis

4. **✍️ Agente escritor: relatorio final**
   - **O que e:** Agente que transforma sintese em relatorio bem escrito e formatado
   - **Por que aprender:** Output precisa ser consumivel por humanos
   - **Conceitos-chave:** Report generation, citations, executive summary

5. **🔍 Agente critico: verificacao de fatos**
   - **O que e:** Agente que verifica afirmacoes, checa fontes e identifica contradicoes
   - **Por que aprender:** Pesquisa sem verificacao e desinformacao
   - **Conceitos-chave:** Fact-checking, source verification, contradiction detection

6. **🔄 Pipeline completo: implementacao**
   - **O que e:** Montagem do sistema completo com LangGraph ou CrewAI
   - **Por que aprender:** Projeto end-to-end que demonstra todas as tecnicas
   - **Conceitos-chave:** Full implementation, testing, iteration

### Recursos:
- [LangChain Academy - Project: Deep Research with LangGraph](https://academy.langchain.com/)
- [Designing Effective Multi-Agent Architectures - O'Reilly](https://www.oreilly.com/radar/designing-effective-multi-agent-architectures/)

---

## Modulo 3.6 - Deploy e infraestrutura para swarms

**Duracao:** ~45 min | **Nivel:** Avancado

### Topicos:

1. **🐳 Containerizacao com Docker**
   - **O que e:** Cada agente em seu container — isolamento, reproducibilidade, seguranca
   - **Por que aprender:** Padrao de deploy para qualquer sistema de producao
   - **Conceitos-chave:** Docker, container per agent, networking

2. **☸️ Kubernetes: orquestracao de containers**
   - **O que e:** Escalar agentes automaticamente baseado em demanda
   - **Por que aprender:** Producao real precisa de auto-scaling
   - **Conceitos-chave:** Pods, scaling, GPU scheduling (NVIDIA Operator)

3. **📊 Observabilidade: rastreamento de agentes**
   - **O que e:** Monitorar cada chamada: tokens, latencia, custo, resultado
   - **Por que aprender:** Sem observabilidade, debugging em producao e impossivel
   - **Conceitos-chave:** Tracing, metrics, dashboards, alertas

4. **💰 Gestao de custos em escala**
   - **O que e:** Calcular, monitorar e otimizar custo por agente e por tarefa
   - **Por que aprender:** Custos de swarms escalam rapido — controle e obrigatorio
   - **Conceitos-chave:** Token budgets, cost per task, provider optimization

5. **🔒 Seguranca em producao**
   - **O que e:** API key management, sandboxing, rate limiting, audit logs
   - **Por que aprender:** Agentes autonomos com acesso a ferramentas sao vetores de risco
   - **Conceitos-chave:** Secret management, least privilege, audit trail

6. **🔄 CI/CD para swarms**
   - **O que e:** Pipeline de deploy automatizado com testes de integracao do swarm
   - **Por que aprender:** Atualizacoes frequentes sem quebrar producao
   - **Conceitos-chave:** Testing pipeline, canary deploy, rollback

### Recursos:
- [Building Production Agent Swarms - AWS](https://dev.to/aws/dev-track-spotlight-building-production-agent-swarms-mastering-industrial-ai-dev311-41b0)
- [The Ultimate Guide to Deploying MAS in Production](https://medium.com/@jalajagr/the-ultimate-guide-to-deploying-multi-agent-systems-in-production-at-scale-24f05d32d0fd)

---

## Modulo 3.7 - Anti-padroes e armadilhas

**Duracao:** ~40 min | **Nivel:** Avancado

### Topicos:

1. **🪤 The Multi-Agent Trap**
   - **O que e:** Especializar demais sem governanca gera sistemas frageis e caros
   - **Por que aprender:** Gartner: 40%+ dos projetos agenticos serao cancelados ate 2027
   - **Conceitos-chave:** Over-engineering, cost escalation, value uncertainty

2. **💸 Custos escalantes nao monitorados**
   - **O que e:** Cada agente consome tokens — sem controle, custos explodem exponencialmente
   - **Por que aprender:** Projetos cancelados por custo sao os mais comuns
   - **Conceitos-chave:** Token budgets, cost alerts, fallback to cheaper models

3. **🤯 Testing theater: testes que nao testam nada**
   - **O que e:** 268 assertions testando texto de prompt em vez de comportamento real (caso real do opencode-swarm)
   - **Por que aprender:** IA adora gerar testes "bonitos" que verificam strings fixas
   - **Conceitos-chave:** Behavioral testing, mutation testing, coverage vs value

4. **🏗️ God Functions: codigo monolitico gerado por IA**
   - **O que e:** Funcoes gigantes que fazem tudo — anti-padrao classico de codigo gerado
   - **Por que aprender:** Agentes frequentemente geram codigo que "funciona" mas e impossivel de manter
   - **Conceitos-chave:** Single responsibility, decomposition, refactoring

5. **🔇 Agentes silenciosos: falhas nao reportadas**
   - **O que e:** Agente encontra erro mas continua sem avisar — resultado parcial parece completo
   - **Por que aprender:** Falhas silenciosas sao mais perigosas que falhas explicitas
   - **Conceitos-chave:** Error propagation, fail-fast, explicit error states

6. **🎯 Governanca cognitiva: o que falta**
   - **O que e:** Reproducibilidade, auditoria, comportamento deterministico — controles para producao real
   - **Por que aprender:** Enterprise nao aceita "funciona as vezes"
   - **Conceitos-chave:** Reproducibility, audit trail, deterministic behavior, compliance

### Recursos:
- [The Multi-Agent Trap - Towards Data Science](https://towardsdatascience.com/the-multi-agent-trap/)
- [opencode-swarm AI_SLOP_REVIEW.md](https://github.com/zaxbysauce/opencode-swarm)

---

## Modulo 3.8 - Futuro dos swarms e proximos passos

**Duracao:** ~35 min | **Nivel:** Todos

### Topicos:

1. **🔮 Tendencias 2026-2027**
   - **O que e:** Federated Agent Networks, Semantic Orchestration, autonomia crescente
   - **Por que aprender:** Antecipar para onde investir tempo de aprendizado
   - **Conceitos-chave:** Federation, semantic matching, increasing autonomy

2. **🌐 Padronizacao: MCP + A2A como infraestrutura**
   - **O que e:** Protocolos abertos se tornam a "Internet dos agentes"
   - **Por que aprender:** Quem dominar protocolos tera vantagem competitiva
   - **Conceitos-chave:** Open standards, interoperability, vendor neutrality

3. **🏢 Adocao enterprise: o que muda**
   - **O que e:** Grandes empresas adotando swarms para automacao de processos complexos
   - **Por que aprender:** Oportunidades profissionais enormes
   - **Conceitos-chave:** Enterprise adoption, compliance, governance

4. **🤖 Agentes que aprendem: fine-tuning para orquestracao**
   - **O que e:** Tecnicas de fine-tuning especificas para melhorar orquestracao em escala
   - **Por que aprender:** Proximo nivel de performance
   - **Conceitos-chave:** Amazon fine-tuning case study, orchestration-specific training

5. **💼 Oportunidades profissionais**
   - **O que e:** Carreiras: engenheiro de swarms, arquiteto multiagente, consultor de automacao
   - **Por que aprender:** Mercado em formacao — quem chegar primeiro tem vantagem
   - **Conceitos-chave:** New roles, certifications, market demand

6. **🚀 Seu roadmap pessoal**
   - **O que e:** Plano pratico: escolha um framework, construa um projeto, itere, contribua
   - **Por que aprender:** Sair do curso com um caminho claro
   - **Conceitos-chave:** Start small, iterate, contribute, grow

### Recursos:
- [The Orchestration of Multi-Agent Systems - arXiv](https://arxiv.org/html/2601.13671v1)
- [Advanced Fine-Tuning for Multi-Agent Orchestration - AWS](https://aws.amazon.com/blogs/machine-learning/advanced-fine-tuning-techniques-for-multi-agent-orchestration-patterns-from-amazon-at-scale/)
- [Agentic AI Certificate - Johns Hopkins](https://online.lifelonglearning.jhu.edu/jhu-certificate-program-agentic-ai)

---

# TRILHA 4: MAO NA MASSA (Amber)

> **Passo a passo: do zero ao projeto entregue com seu proprio swarm**
>
> **Ilustracao principal:** `doc/ChatGPT Image 19...06_27_15.png` (ENXAME DE AGENTES — agindo em paralelo)
>
> Esta trilha e 100% pratica. O aluno segue cada modulo na ordem, e ao final tera instalado, configurado, executado e otimizado seu proprio swarm para construir projetos reais. Baseado diretamente no fluxo demonstrado na aula e na documentacao do oh-my-openagent.

## Modulo 4.1 - Preparando o ambiente

**Duracao:** ~30 min | **Nivel:** Iniciante | **Tipo:** Passo a passo

### Topicos:

1. **💻 Pre-requisitos: o que voce precisa ter**
   - **O que e:** Lista de tudo que precisa estar instalado antes de comecar: terminal, Node.js, Git
   - **Por que aprender:** Sem ambiente correto, nada funciona — evite perder tempo com erros basicos
   - **Conceitos-chave:** Terminal (bash/zsh), Node.js, Git, editor de codigo

2. **📦 Passo 1: instalar o OpenCode**
   - **O que e:** Instalar o OpenCode no seu sistema e verificar que funciona
   - **Por que aprender:** OpenCode e a base onde o swarm vai rodar
   - **Conceitos-chave:**
     ```bash
     # Verificar se OpenCode esta instalado
     opencode --version
     # Se nao estiver, instalar conforme opencode.ai
     ```

3. **🔌 Passo 2: conectar seus provedores de IA**
   - **O que e:** Usar `/connect` dentro do OpenCode para autenticar Claude, OpenAI, Gemini
   - **Por que aprender:** Sem provedores conectados, os agentes nao tem modelos para usar
   - **Conceitos-chave:** `/connect`, `/models`, API keys, provedores gratuitos

4. **📋 Passo 3: verificar modelos disponiveis**
   - **O que e:** Executar `opencode models` para ver todos os modelos acessiveis na sua instalacao
   - **Por que aprender:** Voce precisa saber os nomes exatos para configurar cada agente
   - **Conceitos-chave:**
     ```bash
     opencode models
     # Lista todos: anthropic/claude-opus-4-6, openai/gpt-5.3-codex,
     # opencode/big-pickle (gratuito), etc.
     ```

5. **🔧 Passo 4: instalar o Bun**
   - **O que e:** Instalar o runtime Bun — obrigatorio para o oh-my-openagent
   - **Por que aprender:** O OMO nao funciona sem Bun — e o erro mais comum de quem comeca
   - **Conceitos-chave:**
     ```bash
     curl -fsSL https://bun.sh/install | bash
     # Fechar e reabrir terminal
     bun --version  # Verificar
     ```

6. **✅ Checkpoint: tudo pronto?**
   - **O que e:** Checklist de verificacao — todos os pre-requisitos confirmados
   - **Por que aprender:** Seguir em frente sem o ambiente pronto gera frustracoes desnecessarias
   - **Conceitos-chave:**
     ```markdown
     Checklist:
     - [ ] OpenCode instalado e abrindo
     - [ ] Pelo menos 1 provedor conectado (/models mostra modelos)
     - [ ] Bun instalado (bun --version funciona)
     - [ ] Pasta do projeto criada
     ```

### Recursos:
- [OpenCode - opencode.ai](http://opencode.ai)
- [Bun - bun.sh](http://bun.sh)

---

## Modulo 4.2 - Instalando o oh-my-openagent

**Duracao:** ~25 min | **Nivel:** Iniciante | **Tipo:** Passo a passo

### Topicos:

1. **🎯 Escolher: instalacao global ou por projeto**
   - **O que e:** Global ativa em todos os projetos; por projeto ativa so naquela pasta
   - **Por que aprender:** Escolher errado pode atrapalhar outros projetos ou limitar o uso
   - **Conceitos-chave:**
     | | Global | Por Projeto |
     |---|---|---|
     | Ativa em | Todos os projetos | So nesse |
     | Ideal para | Uso pessoal diario | Demos, aulas |

2. **⚡ Passo 1: identificar suas assinaturas**
   - **O que e:** Verificar quais provedores voce tem (Claude, OpenAI, Gemini, Copilot, so gratuitos)
   - **Por que aprender:** O comando de instalacao muda conforme seus provedores
   - **Conceitos-chave:** Claude + Gemini (mais comum), so Claude, Claude + OpenAI, so gratuitos

3. **📦 Passo 2: executar o instalador**
   - **O que e:** Rodar o comando correto para seu caso
   - **Por que aprender:** E a unica etapa de instalacao — um comando faz tudo
   - **Conceitos-chave:**
     ```bash
     # Caso mais comum: Claude + Gemini (Antigravity)
     bunx oh-my-opencode install --no-tui --claude=yes --gemini=yes --copilot=no --opencode-zen=yes

     # So Claude
     bunx oh-my-opencode install --no-tui --claude=yes --gemini=no --copilot=no --opencode-zen=yes

     # Claude + ChatGPT Plus
     bunx oh-my-opencode install --no-tui --claude=yes --openai=yes --gemini=no --copilot=no

     # So modelos gratuitos
     bunx oh-my-opencode install --no-tui --claude=no --openai=no --gemini=no --copilot=no --opencode-zen=yes
     ```

4. **🔍 Passo 3: verificar a instalacao**
   - **O que e:** Confirmar que o plugin foi registrado corretamente
   - **Por que aprender:** Se nao verificar agora, voce descobre o problema no pior momento
   - **Conceitos-chave:**
     ```bash
     cat ~/.config/opencode/opencode.json
     # Deve mostrar "oh-my-opencode" no array de plugins
     ```

5. **🚀 Passo 4: abrir OpenCode e conferir a mudanca**
   - **O que e:** Ao abrir OpenCode, os modos Build/Plan desaparecem e surgem Sisyphus, Hephaestus, Prometheus
   - **Por que aprender:** Confirmacao visual de que o swarm esta ativo
   - **Conceitos-chave:**
     ```bash
     cd seu-projeto
     opencode
     # Agora voce ve: Sisyphus, Hephaestus, Plan Builder, Plan Executor
     ```

6. **🛠️ Solucao de problemas comuns**
   - **O que e:** Os 5 erros mais comuns na instalacao e como resolver cada um
   - **Por que aprender:** Nao ficar travado por erros simples
   - **Conceitos-chave:** bunx not found, plugin nao aparece, modelos com prefixo errado, Sisyphus generico, agentes nao paralelos

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 4.3 - Configurando os modelos de cada agente

**Duracao:** ~30 min | **Nivel:** Iniciante-Intermediario | **Tipo:** Passo a passo

### Topicos:

1. **🧩 Entender a estrategia: modelo certo para cada papel**
   - **O que e:** Agentes criticos (Sisyphus, Prometheus) precisam de modelos potentes; agentes de suporte podem usar gratuitos
   - **Por que aprender:** Otimizar custo sem sacrificar qualidade — a diferenca pode ser 10x no preco
   - **Conceitos-chave:**
     | Agente | Funcao | Modelo Recomendado | Custo |
     |--------|--------|--------------------|-------|
     | Sisyphus | Orquestrador | claude-opus-4-6 | Pago |
     | Prometheus | Planejador | claude-sonnet-4-5 | Pago |
     | Hephaestus | Executor | gpt-5.3-codex | Pago |
     | Oracle | Debug | opencode/big-pickle | Gratuito |
     | Librarian | Pesquisa | opencode/gpt-5-nano | Gratuito |
     | Explore | Explorador | opencode/gpt-5-nano | Gratuito |

2. **📄 Passo 1: criar o arquivo de configuracao**
   - **O que e:** Criar `.opencode/oh-my-opencode.jsonc` na raiz do projeto
   - **Por que aprender:** E onde voce define qual modelo cada agente usa
   - **Conceitos-chave:**
     ```bash
     mkdir -p .opencode
     # Criar/editar .opencode/oh-my-opencode.jsonc
     ```

3. **✍️ Passo 2: definir os modelos**
   - **O que e:** Escrever o JSON com o mapeamento agente → modelo
   - **Por que aprender:** Hands-on — voce faz agora
   - **Conceitos-chave:**
     ```json
     {
       "sisyphus":   { "model": "anthropic/claude-opus-4-6" },
       "hephaestus": { "model": "openai/gpt-5.3-codex" },
       "prometheus": { "model": "anthropic/claude-sonnet-4-5" },
       "oracle":     { "model": "opencode/big-pickle" },
       "librarian":  { "model": "opencode/gpt-5-nano" },
       "explore":    { "model": "opencode/gpt-5-nano" }
     }
     ```

4. **🔀 Passo 3: trocar modelos em tempo real**
   - **O que e:** Se acabar creditos de um provedor, basta editar o arquivo e continuar
   - **Por que aprender:** Na aula real, os creditos de Claude acabaram e trocamos para GPT sem perder o progresso
   - **Conceitos-chave:** Hot-swap, sem reiniciar, fallback de provider

5. **💰 Passo 4: estrategia para quem so tem gratuitos**
   - **O que e:** Configuracao otimizada usando apenas modelos gratuitos do OpenCode
   - **Por que aprender:** Nem todos tem assinaturas pagas — funciona tambem
   - **Conceitos-chave:**
     ```json
     {
       "sisyphus":   { "model": "opencode/big-pickle" },
       "hephaestus": { "model": "opencode/big-pickle" },
       "prometheus": { "model": "opencode/big-pickle" }
     }
     ```
     > Funciona, mas a qualidade e significativamente menor sem Claude

6. **✅ Checkpoint: configuracao validada**
   - **O que e:** Abrir OpenCode e confirmar que cada agente mostra o modelo correto
   - **Por que aprender:** Validar antes de comecar a executar
   - **Conceitos-chave:** Verificar na interface que modelos mudaram, testar um comando simples

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 4.4 - Primeira execucao: modo linguagem natural

**Duracao:** ~35 min | **Nivel:** Iniciante | **Tipo:** Passo a passo

### Topicos:

1. **🎯 Escolher uma tarefa simples para comecar**
   - **O que e:** Comecar com algo pequeno — uma pagina HTML basica, um componente, um script
   - **Por que aprender:** Primeira execucao deve ser simples para entender o fluxo sem complexidade
   - **Conceitos-chave:** Start small, observar o comportamento, aprender o fluxo

2. **💬 Passo 1: descrever a tarefa em linguagem natural**
   - **O que e:** No chat do OpenCode (Sisyphus), escrever o que quer em portugues claro
   - **Por que aprender:** E o modo mais direto — sem comandos especiais
   - **Conceitos-chave:**
     ```text
     Crie uma pagina HTML simples com titulo "Meu Primeiro Swarm",
     um paragrafo explicando o que sao swarms e um botao que
     mostra um alerta. Use CSS inline, sem frameworks.
     ```

3. **👀 Passo 2: observar o Sisyphus em acao**
   - **O que e:** Ver como o orquestrador decide qual agente usar e delega a tarefa
   - **Por que aprender:** Entender o fluxo de roteamento e delegacao
   - **Conceitos-chave:** Sisyphus analisa → categoriza (Quick/Deep/UltraBrain) → delega

4. **🔍 Passo 3: acompanhar os subagentes**
   - **O que e:** Clicar nos indicadores de subagentes para ver o que cada um esta fazendo
   - **Por que aprender:** Transparencia — voce ve exatamente quem faz o que
   - **Conceitos-chave:** Subagent indicators, logs, progresso

5. **📂 Passo 4: verificar o resultado**
   - **O que e:** Abrir os arquivos gerados e testar no navegador
   - **Por que aprender:** Validar que o swarm entregou o esperado
   - **Conceitos-chave:** Abrir no navegador, verificar console (zero erros), revisar codigo

6. **📝 O que aprendemos nesta primeira execucao**
   - **O que e:** Reflexao sobre o fluxo: Sisyphus recebeu → categorizou → delegou → agente executou → resultado
   - **Por que aprender:** Consolidar o modelo mental antes de execucoes mais complexas
   - **Conceitos-chave:** Fluxo basico, roteamento automatico, resultado sem intervencao

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 4.5 - Modo Prometheus: entrevista antes de executar

**Duracao:** ~45 min | **Nivel:** Intermediario | **Tipo:** Passo a passo

### Topicos:

1. **📋 Por que a entrevista faz toda a diferenca**
   - **O que e:** Prometheus extrai requisitos completos ANTES de uma linha de codigo — como um engenheiro real
   - **Por que aprender:** "A entrevista previa faz toda a diferenca na qualidade do resultado" (conselho-chave da aula)
   - **Conceitos-chave:** Discovery, requirements gathering, escopo claro

2. **🔄 Passo 1: trocar para o agente Prometheus**
   - **O que e:** Pressionar Tab no OpenCode para mudar de Sisyphus para Prometheus (Plan Builder)
   - **Por que aprender:** Prometheus so e ativado quando voce muda para ele manualmente
   - **Conceitos-chave:**
     ```text
     [Tab] → Selecionar Prometheus / Plan Builder
     ```

3. **✍️ Passo 2: descrever o projeto e pedir entrevista**
   - **O que e:** Escrever o objetivo geral e pedir que Prometheus entreviste antes de comecar
   - **Por que aprender:** O prompt inicial define a qualidade de toda a entrevista
   - **Conceitos-chave:**
     ```text
     Quero construir uma landing page profissional para uma
     consultoria de IA. Me entreviste antes de comecar.
     ```

4. **🗣️ Passo 3: responder as perguntas do Prometheus**
   - **O que e:** Prometheus pergunta sobre idioma, secoes, tom de voz, stack, conteudo, equipe, formulario
   - **Por que aprender:** Cada resposta refina o plano — quanto mais contexto, melhor o resultado
   - **Conceitos-chave:** Perguntas sobre: nome, servicos, publico-alvo, idioma, tom de voz, secoes desejadas, stack tecnico, formulario, referencias visuais

5. **📊 Passo 4: revisar o resumo e confirmar**
   - **O que e:** Prometheus mostra resumo de tudo que coletou e pede confirmacao
   - **Por que aprender:** Ultima chance de corrigir antes da execucao
   - **Conceitos-chave:**
     ```text
     Prometheus mostra:
     - Nome: [consultoria]
     - Servicos: [lista]
     - Secoes: [10 secoes]
     - Stack: [Next.js + Tailwind]
     - Tom: [profissional mas proximo]
     → "Confirma? Arrancamos com o plano de implementacao?"
     → Responder: "Sim, correto"
     ```

6. **🚀 Passo 5: executar com /start-work**
   - **O que e:** Digitar `/start-work` para que Sisyphus assuma e execute o plano com todos os agentes em paralelo
   - **Por que aprender:** E o momento em que o swarm comeca a trabalhar de verdade
   - **Conceitos-chave:**
     ```text
     /start-work
     # Sisyphus assume → delega para agentes em paralelo
     # Plan Executor ativa → Wave 1, Wave 2, Wave 3...
     # Voce nao precisa fazer mais nada
     ```

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 4.6 - Modo ultrawork: execucao autonoma completa

**Duracao:** ~40 min | **Nivel:** Intermediario | **Tipo:** Passo a passo

### Topicos:

1. **⚡ Quando usar ultrawork**
   - **O que e:** Ideal quando voce ja sabe exatamente o que quer e prioriza velocidade
   - **Por que aprender:** "ultrawork e perfeito quando voce ja sabe o que quer" (conselho-chave)
   - **Conceitos-chave:** Clareza do objetivo, velocidade, sem entrevista

2. **🔥 Passo 1: ativar o ultrawork**
   - **O que e:** Escrever `ultrawork` ou `ulw` no chat do Sisyphus
   - **Por que aprender:** Um unico comando ativa toda a equipe de agentes
   - **Conceitos-chave:**
     ```text
     ultrawork
     # Resposta: "Ultra Work Mode Enabled. Diga o que quer."
     ```

3. **📝 Passo 2: descrever a tarefa completa**
   - **O que e:** Dar toda a informacao de uma vez — quanto mais detalhado, melhor
   - **Por que aprender:** Sem entrevista, tudo que o swarm sabe vem do seu prompt
   - **Conceitos-chave:**
     ```text
     Construa uma landing page com:
     - Hero com titulo "SoluTech IA" e subtitulo
     - Secao de 6 servicos com icones
     - Como trabalhamos (processo em 4 etapas)
     - Depoimentos de 3 clientes
     - FAQ com 5 perguntas
     - Formulario de contato (nome, email, empresa, telefone, mensagem)
     - Footer com links e redes sociais
     Stack: HTML, CSS e JavaScript vanilla. Tema escuro.
     ```

4. **🔄 Passo 3: observar a execucao paralela**
   - **O que e:** Multiplos agentes trabalhando simultaneamente — cada um em sua zona segura
   - **Por que aprender:** Ver o paralelismo real em acao
   - **Conceitos-chave:** Agentes em background, zonas de arquivo exclusivas, sem conflitos

5. **☕ Passo 4: esperar (ir tomar um cafe)**
   - **O que e:** "Voce liga e vai tomar um cafe" — o sistema se autocorrige, testa e chega ao final sozinho
   - **Por que aprender:** A autonomia e o maior beneficio do ultrawork
   - **Conceitos-chave:** Auto-correcao, teste local automatico, zero intervencao manual

6. **✅ Passo 5: revisar o resultado final**
   - **O que e:** Verificar a pagina gerada, testar no navegador, confirmar zero erros no console
   - **Por que aprender:** Mesmo com execucao autonoma, revisao humana final e essencial
   - **Conceitos-chave:**
     ```text
     # O sistema abre localhost:3000 automaticamente
     # Verificar: todas as secoes presentes, formulario funcional,
     # console sem erros, responsivo, politica de privacidade
     ```

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 4.7 - Comandos avancados e tecnicas de otimizacao

**Duracao:** ~35 min | **Nivel:** Intermediario | **Tipo:** Passo a passo

### Topicos:

1. **🔄 /ulw-loop: loop ate a perfeicao**
   - **O que e:** Modo que nao para ate o resultado ficar perfeito — autocorrecao em loop
   - **Por que aprender:** Para projetos onde qualidade e mais importante que velocidade
   - **Conceitos-chave:**
     ```text
     /ulw-loop
     # O sistema executa, revisa, corrige, executa de novo...
     # Ate atingir zero erros e qualidade satisfatoria
     ```

2. **📂 /init-deep: contexto profundo do projeto**
   - **O que e:** Gera arquivo AGENTS.md em cada pasta do projeto para otimizar contexto dos agentes
   - **Por que aprender:** Em projetos grandes, melhora drasticamente a qualidade das decisoes dos agentes
   - **Conceitos-chave:**
     ```text
     /init-deep
     # Cria AGENTS.md em cada diretorio
     # Agentes entendem a estrutura do projeto inteiro
     ```

3. **🔍 /review: revisao antes do deploy**
   - **O que e:** Revisa mudancas do ultimo commit ou branch antes de fazer merge
   - **Por que aprender:** Ultima camada de seguranca antes de entregar
   - **Conceitos-chave:**
     ```text
     /review
     # Agente revisor analisa diff, busca problemas,
     # sugere melhorias
     ```

4. **🖼️ Multimodal Looker: de imagem para codigo**
   - **O que e:** Fornecer uma imagem/mockup e o agente visual converte em codigo
   - **Por que aprender:** Acelera drasticamente a implementacao de designs
   - **Conceitos-chave:** Screenshot, mockup, Figma export → HTML/CSS gerado

5. **🔧 Trocar provedor no meio da execucao**
   - **O que e:** Se creditos acabarem, editar o jsonc e continuar sem perder progresso
   - **Por que aprender:** Aconteceu na aula real — creditos de Claude acabaram, trocamos para GPT
   - **Conceitos-chave:**
     ```text
     # 1. Editar .opencode/oh-my-opencode.jsonc
     # 2. Trocar modelo do agente que precisa
     # 3. Salvar — sistema continua automaticamente
     ```

6. **📊 Monitorando custo e tokens**
   - **O que e:** Acompanhar quanto cada agente esta consumindo para otimizar
   - **Por que aprender:** Evitar surpresas na conta
   - **Conceitos-chave:** Token usage, provider dashboard, custo por agente

### Recursos:
- Conteudo baseado no material do curso

---

## Modulo 4.8 - Projeto guiado completo: do zero ao deploy

**Duracao:** ~90 min | **Nivel:** Intermediario | **Tipo:** Projeto completo

### Topicos:

1. **🎯 Definicao do projeto: landing page para sua marca**
   - **O que e:** O aluno escolhe um tema real (sua empresa, projeto pessoal, portfolio) e constroi com swarm
   - **Por que aprender:** Projeto proprio gera motivacao e resultado util de verdade
   - **Conceitos-chave:** Escolher tema, definir 5-10 secoes, escolher stack

2. **📋 Fase 1: Entrevista com Prometheus (15 min)**
   - **O que e:** Seguir o fluxo completo: Tab → Prometheus → descrever projeto → responder perguntas → confirmar
   - **Por que aprender:** Repetir o processo da aula com seu proprio conteudo
   - **Conceitos-chave:**
     ```text
     Fluxo completo:
     1. [Tab] → Prometheus
     2. "Quero construir [seu projeto]. Me entreviste."
     3. Responder todas as perguntas
     4. Revisar resumo → Confirmar
     5. /start-work
     ```

3. **🚀 Fase 2: Execucao do swarm (30-45 min)**
   - **O que e:** O swarm executa em paralelo — waves de implementacao, revisao e teste automaticos
   - **Por que aprender:** Vivenciar o poder do sistema multiagente no seu projeto
   - **Conceitos-chave:** Wave 1 (estrutura), Wave 2 (conteudo), Wave 3 (estilo), Wave 4 (interatividade), Wave 5 (revisao), Wave 6 (polish)

4. **🔍 Fase 3: Revisao e ajustes (15 min)**
   - **O que e:** Revisar resultado, pedir ajustes pontuais, usar /review para validacao final
   - **Por que aprender:** Swarm entrega 90% — os 10% finais sao refinamento humano
   - **Conceitos-chave:**
     ```text
     # Ajustes pontuais em linguagem natural:
     "Mude a cor do hero para azul escuro"
     "Adicione mais um depoimento"
     "O formulario precisa de campo telefone"
     ```

5. **✅ Fase 4: Validacao final e checklist**
   - **O que e:** Checklist completo de qualidade antes de considerar o projeto pronto
   - **Por que aprender:** Processo sistematico garante qualidade consistente
   - **Conceitos-chave:**
     ```markdown
     Checklist Final:
     - [ ] Todas as secoes presentes e com conteudo
     - [ ] Formulario funcional (todos os campos)
     - [ ] Responsivo (testar em mobile)
     - [ ] Zero erros no console do navegador
     - [ ] Links funcionando (footer, redes sociais)
     - [ ] Politica de privacidade presente
     - [ ] Performance aceitavel (carregamento rapido)
     - [ ] Texto sem erros de portugues
     ```

6. **🏆 Resultado: o que voce construiu**
   - **O que e:** Reflexao final: voce deu um prompt, respondeu perguntas, tomou um cafe e tem um projeto completo
   - **Por que aprender:** Consolidar a experiencia e planejar proximos projetos mais ambiciosos
   - **Conceitos-chave:**
     ```text
     O que voce aprendeu:
     ✅ Instalar e configurar ambiente completo
     ✅ Escolher e atribuir modelos por agente
     ✅ Usar os 3 modos (natural, Prometheus, ultrawork)
     ✅ Acompanhar execucao paralela de agentes
     ✅ Trocar modelos em tempo real
     ✅ Revisar e ajustar resultado
     ✅ Entregar projeto funcional do zero

     Proximo desafio:
     → Construir um projeto mais complexo (app, dashboard, API)
     → Experimentar com CrewAI ou LangGraph (Trilha 2)
     → Criar seu proprio swarm customizado (Trilha 3)
     ```

### Recursos:
- Conteudo baseado no material do curso

---

# RECURSOS COMPLEMENTARES

## Cursos Online Recomendados

| Curso | Plataforma | Nivel | Gratuito? |
|-------|-----------|-------|-----------|
| Agentic AI (Andrew Ng) | DeepLearning.AI | Iniciante | Sim |
| Introduction to LangGraph | LangChain Academy | Iniciante | Sim |
| Multi AI Agent Systems with crewAI | DeepLearning.AI | Intermediario | Sim |
| A2A: The Agent2Agent Protocol | DeepLearning.AI | Intermediario | Sim |
| AI Agents Bootcamp | Zero To Mastery | Avancado | Pago |
| Agentic AI Certificate | Johns Hopkins / Coursera | Profissional | Pago |

## Documentacao Oficial (Bookmark Obrigatorio)

- [CrewAI Docs](https://docs.crewai.com)
- [LangGraph Docs](https://docs.langchain.com/oss/python/langgraph/overview)
- [AutoGen Docs](https://microsoft.github.io/autogen/stable/)
- [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/)
- [OpenAI Swarm](https://github.com/openai/swarm)
- [Swarms Framework](https://docs.swarms.world/en/latest/)
- [A2A Protocol](https://a2a-protocol.org/latest/)

## Repositorios de Referencia

- [opencode-swarm](https://github.com/zaxbysauce/opencode-swarm) — 828 commits, 18 design decisions, referencia arquitetural
- [oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent) — 41k stars, plugin multiagente para OpenCode
- [crewAI-examples](https://github.com/crewAIInc/crewAI-examples) — Exemplos oficiais CrewAI
- [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph) — Framework de grafos

---

# ESTRUTURA DE ARQUIVOS DO CURSO

```
enxamesagentes/
├── index.html                              ← Pagina principal do curso
├── trilhas/
│   ├── fundamentos.html                    ← Trilha 1 (Emerald)
│   ├── tecnicas.html                       ← Trilha 2 (Blue)
│   ├── pratica-avancada.html               ← Trilha 3 (Purple)
│   └── mao-na-massa.html                   ← Trilha 4 (Amber)
├── modulos/
│   ├── fundamentos/
│   │   ├── modulo-01.html through 08.html  ← 8 modulos Trilha 1
│   ├── tecnicas/
│   │   ├── modulo-01.html through 08.html  ← 8 modulos Trilha 2
│   ├── pratica-avancada/
│   │   ├── modulo-01.html through 08.html  ← 8 modulos Trilha 3
│   └── mao-na-massa/
│       ├── modulo-01.html through 08.html  ← 8 modulos Trilha 4
├── downloads/
│   ├── fundamentos/
│   │   ├── modulo-01.md through 08.md
│   ├── tecnicas/
│   │   ├── modulo-01.md through 08.md
│   ├── pratica-avancada/
│   │   ├── modulo-01.md through 08.md
│   └── mao-na-massa/
│       ├── modulo-01.md through 08.md
├── doc/                                    ← Conteudo fonte (PRIVADO - no .gitignore)
├── js/
│   └── app.js                              ← JavaScript compartilhado
└── CURSO_ENXAMES_PLANO.md                  ← Este documento
```

## Tailwind Config para este Curso

```javascript
tailwind.config = {
  darkMode: 'class',
  theme: {
    extend: {
      colors: {
        'trilha-1': '#10B981',   // Emerald — Fundamentos
        'trilha-2': '#3B82F6',   // Blue — Tecnicas
        'trilha-3': '#9b59b6',   // Purple — Pratica Avancada
        'trilha-4': '#F59E0B',   // Amber — Mao na Massa
        success: '#22C55E',
        warning: '#F59E0B',
        error: '#EF4444',
      },
      fontFamily: {
        sans: ['Inter', '-apple-system', 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'sans-serif'],
      },
    }
  }
}
```

## Seguir Padrao PADRAO_MODULOS_INTERATIVOS.md

Cada modulo segue o padrao ja estabelecido:
- ✅ 3 botoes: Modal (resumo), Completo (pagina full), Download (MD)
- ✅ 6-8 topicos clicaveis expandiveis
- ✅ Cada topico: 3 respostas (O que e, Por que, Conceitos)
- ✅ 1 modal com resumo de 300-500 palavras
- ✅ Dark mode + responsivo + Tailwind CSS

---

# PROXIMOS PASSOS

1. **✅ Plano aprovado** → Revisar e validar estrutura
2. **Gerar index.html** → Pagina principal com hero usando ilustracao "ENXAME DE AGENTES"
3. **Gerar paginas de trilhas** → 3 paginas com 8 modulos cada
4. **Gerar paginas de modulos** → 24 paginas HTML completas
5. **Gerar downloads MD** → 24 arquivos Markdown para download
6. **Revisao final** → Validar links, modais, navegacao

---

**Versao:** 1.0
**Ultima atualizacao:** 2026-03-19
