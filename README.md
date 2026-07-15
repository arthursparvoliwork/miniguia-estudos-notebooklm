# 🧠 Miniguia de Estudos: Fundamentos de IA Generativa e Engenharia de Prompts

> Projeto desenvolvido para o desafio "Explorando IA como Ferramenta de Aprendizagem Ativa" da DIO, utilizando o NotebookLM do Google para construir um Caderno Temático de estudos.

---

## 🎯 Contexto e Objetivos

### Assunto escolhido
Escolhi estudar Inteligência Artificial Generativa e Engenharia de Prompts, pois é um tema que impacta diretamente minha rotina como estudante de tecnologia: entender como os modelos de linguagem (LLMs) funcionam e como escrever prompts melhores me ajuda a extrair mais valor de qualquer ferramenta de IA que eu use no dia a dia  incluindo o próprio NotebookLM usado nesta atividade.

### Objetivos de estudo
- Compreender os conceitos fundamentais por trás dos LLMs (tokens, contexto, temperatura, etc.).
- Entender as principais técnicas de engenharia de prompts (zero-shot, few-shot, chain-of-thought, system prompting).
- Aprender a aplicar essas técnicas de forma prática no meu dia a dia (estudos, trabalho, projetos pessoais).
- Desenvolver um repertório de prompts reutilizáveis para revisar o conteúdo no futuro.
- Praticar curadoria de fontes confiáveis e pensamento crítico ao interagir com uma IA.

---

## 📚 Curadoria de Fontes

Fontes abertas selecionadas e carregadas no NotebookLM (todas gratuitas, sem necessidade de login para acesso ao conteúdo):

| # | Fonte | Tipo | Link |
|---|-------|------|------|
| 1 | Prompt Engineering — Lee Boonstra (Google/Kaggle Whitepaper) | PDF | https://www.kaggle.com/whitepaper-prompt-engineering |
| 2 | Foundational Large Language Models & Text Generation — Google/Kaggle Whitepaper | PDF | https://www.kaggle.com/whitepaper-foundational-llm-and-text-generation |
| 3 | Prompt Engineering Overview — Documentação oficial da Anthropic | Texto/Web | https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview |
| 4 | Gemini for Google Workspace — Prompting Guide 101 | PDF | https://services.google.com/fh/files/misc/gemini_for_workspace_prompt_guide_october_2024_digital_final.pdf |
| 5 | A Practical Guide to Building Agents — OpenAI | PDF | https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf |

Critério de seleção: priorizei materiais publicados diretamente pelas próprias empresas desenvolvedoras de LLMs (Google, Anthropic, OpenAI), por serem fontes primárias, gratuitas e tecnicamente confiáveis, cobrindo tanto a teoria (whitepapers) quanto a prática (guias de prompting).

---

## 🔬 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Documentação do processo de perguntas feitas ao NotebookLM, variações testadas e dificuldades encontradas.

### Prompt 1 — Pergunta ampla de abertura
Prompt: "Com base nas fontes carregadas, explique de forma simples o que é engenharia de prompts e por que ela é importante."

- Resultado: resposta genérica demais, misturando conceitos de LLM em geral com prompting.
- Dificuldade: o NotebookLM tende a responder de forma ampla quando a pergunta é aberta, sem aproveitar bem a especificidade das fontes.
- Ajuste feito: dividi a pergunta em duas menores e pedi para citar explicitamente de qual fonte cada informação vinha.

### Prompt 2 — Refinamento com pedido de citação
Prompt: "Liste as 4 principais técnicas de prompting descritas nas fontes (zero-shot, few-shot, chain-of-thought, system prompting), explique cada uma em 2 linhas e indique em qual documento cada técnica aparece."

- Resultado: resposta muito mais estruturada e útil, com referência direta às fontes (citações automáticas do NotebookLM).
- Aprendizado: pedir explicitamente estrutura (lista, comparação, tabela) e rastreabilidade da fonte melhora muito a qualidade da resposta.

### Prompt 3 — Teste de "raciocínio guiado" (chain-of-thought)
Prompt: "Aja como um professor de IA. Explique passo a passo como eu escreveria um prompt few-shot para classificar sentimentos de comentários de clientes, usando um exemplo prático."

- Resultado: ótima resposta prática, com exemplo replicável.
- Dificuldade encontrada: na primeira tentativa (sem o "aja como um professor"), a resposta foi mais teórica e menos aplicada. Adicionar um papel (role prompting) mudou completamente o tom e a utilidade da resposta.

### Prompt 4 — Teste de limite (o que a IA erra)
Prompt: "Quais são as desvantagens da engenharia de prompts que as fontes não mencionam?"

- Resultado: o NotebookLM corretamente indicou que não podia responder com confiança, pois a pergunta pedia informação fora das fontes carregadas.
- Aprendizado importante: essa é uma característica valiosa do NotebookLM — ele se recusa a "alucinar" além do material fornecido, o que reforça a importância de uma boa curadoria de fontes.

### Principais dificuldades gerais (troubleshooting)
- Perguntas muito abertas geram respostas rasas → solução: ser específico e pedir formato de saída (lista, tabela, comparação).
- Respostas às vezes repetem trechos genéricos de uma única fonte → solução: pedir explicitamente para cruzar informações de 2+ fontes.
- Termos técnicos em inglês (ex: "few-shot") às vezes não eram traduzidos → solução: pedir explicitamente "responda em português e traduza termos técnicos, mantendo o termo original entre parênteses".

---

## 📖 Miniguia de Estudo (Entrega Final)

### 1. Resumos estruturados

O que é um LLM (Large Language Model)?
Um modelo de linguagem grande é um sistema de IA treinado com enormes volumes de texto para prever a próxima palavra (ou token) de uma sequência. A partir desse treinamento, ele "aprende" padrões de linguagem, fatos e raciocínio que permitem gerar texto coerente, responder perguntas e seguir instruções.

O que é Engenharia de Prompts?
É a prática de estruturar as instruções (prompts) dadas a um LLM para obter respostas mais precisas, relevantes e úteis. Não é sobre "adivinhar palavras mágicas", mas sobre comunicação clara: dar contexto, exemplos, formato esperado e critérios de qualidade.

Principais técnicas de prompting:
- Zero-shot: pedir uma tarefa diretamente, sem exemplos. Rápido, mas menos preciso para tarefas complexas.
- Few-shot: fornecer alguns exemplos do padrão desejado antes de pedir a tarefa. Melhora muito a consistência do formato de saída.
- System prompting: definir um contexto/papel geral para a IA (ex: "você é um especialista em..."), orientando o tom e o escopo de todas as respostas seguintes.
- Chain-of-thought (Cadeia de pensamento): pedir para a IA "pensar passo a passo" antes de dar a resposta final, o que melhora o raciocínio em tarefas lógicas e matemáticas.

Boas práticas gerais:
- Ser específico sobre o formato de saída desejado (lista, tabela, JSON, tamanho do texto).
- Fornecer contexto suficiente, mas evitar excesso de informação irrelevante.
- Iterar: o primeiro prompt raramente é o melhor — refinar com base na resposta obtida.
- Testar variações (com e sem exemplos, com e sem papel definido) para entender o que funciona melhor para cada tarefa.

### 2. Glossário

| Termo | Definição |
|-------|-----------|
| LLM (Large Language Model) | Modelo de linguagem treinado em grandes volumes de texto para gerar e compreender linguagem natural. |
| Prompt | Instrução ou pergunta enviada a um modelo de IA para obter uma resposta. |
| Token | Unidade mínima de texto processada por um LLM (pode ser uma palavra, parte de uma palavra ou pontuação). |
| Zero-shot prompting | Técnica em que se pede uma tarefa sem fornecer exemplos prévios. |
| Few-shot prompting | Técnica em que se fornecem exemplos do resultado esperado antes da tarefa real. |
| System prompt | Instrução inicial que define o papel, tom ou contexto geral da IA durante a conversa. |
| Chain-of-thought (CoT) | Técnica que induz o modelo a explicar seu raciocínio passo a passo antes da resposta final. |
| Temperatura | Parâmetro que controla a aleatoriedade/criatividade das respostas de um modelo (valores baixos = mais previsível). |
| Alucinação | Quando a IA gera informação incorreta ou inventada com aparência de fato verdadeiro. |
| NotebookLM | Ferramenta do Google que permite carregar fontes próprias e conversar com uma IA restrita a esse material. |

### 3. Prompts reutilizáveis (para futuras revisões)

1. "Resuma os principais conceitos da fonte [X] em uma lista de tópicos, para revisão rápida."
2. "Crie 5 perguntas de múltipla escolha sobre [tema], baseadas apenas nas fontes carregadas, e me dê o gabarito ao final."
3. "Compare os conceitos de [conceito A] e [conceito B] mencionados nas fontes, em formato de tabela."
4. "Aja como um professor e me explique [conceito] como se eu tivesse acabado de conhecer o assunto, com um exemplo prático."
5. "Com base apenas nas fontes carregadas, quais pontos ainda não ficaram claros ou têm informações conflitantes entre os documentos?"
6. "Gere um roteiro de podcast de 3 minutos explicando [tema] de forma didática, usando as fontes carregadas como base."

---

## 🛠️ Ferramentas utilizadas
- NotebookLM — para curadoria de fontes e geração de respostas contextualizadas.
- GitHub — para versionamento e publicação do portfólio.

## ✅ Checklist do desafio
- [x] Contexto e objetivos de estudo definidos
- [x] 5 fontes abertas curadas e listadas
- [x] Prompts testados e documentados (com troubleshooting)
- [x] Miniguia final com resumos, glossário e prompts reutilizáveis

---

*Projeto feito como parte do bootcamp/desafio de projeto da DIO.*
