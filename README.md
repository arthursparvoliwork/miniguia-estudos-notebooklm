# Meu Caderno de Estudos: Aprendendo sobre IA e Prompts

Esse repositório é o resultado de um desafio da DIO onde a gente usa o NotebookLM pra estudar um assunto usando IA como ferramenta de aprendizado.

---

## Por que escolhi esse tema

Resolvi estudar sobre Inteligência Artificial Generativa e como escrever prompts melhores. Uso IA praticamente todo dia (pra estudar, pra trabalhar, pra tirar dúvida), mas percebi que muitas vezes eu não sabia perguntar direito pra ela, e as respostas saíam meio rasas. Então pensei: por que não aprender de verdade como isso funciona?

### O que eu queria aprender
- Entender como os modelos de IA (tipo ChatGPT, Gemini, Claude) funcionam por trás dos panos
- Aprender técnicas pra escrever prompts melhores e ter respostas mais úteis
- Guardar isso tudo de um jeito que eu consiga revisar depois

---

## As fontes que usei

Subi esses materiais no NotebookLM pra estudar:

1. Prompt Engineering - um guia da Google/Kaggle sobre como escrever prompts (https://www.kaggle.com/whitepaper-prompt-engineering)
2. Foundational Large Language Models & Text Generation - outro material da Google explicando como os LLMs funcionam (https://www.kaggle.com/whitepaper-foundational-llm-and-text-generation)
3. Guia de prompt engineering da Anthropic, empresa que faz o Claude (https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview)
4. Guia de prompts do Google Workspace com Gemini (https://services.google.com/fh/files/misc/gemini_for_workspace_prompt_guide_october_2024_digital_final.pdf)
5. Um guia da OpenAI sobre como construir agentes de IA (https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf)

Escolhi esses porque são direto das empresas que criam essas IAs, então é informação confiável e de graça pra qualquer um acessar.

---

## Testando prompts no NotebookLM

Fui fazendo perguntas pro NotebookLM e fui ajustando conforme via o que funcionava melhor.

**Primeira tentativa:** perguntei de forma bem genérica "o que é engenharia de prompts e por que é importante". A resposta veio meio vaga, misturando várias coisas.

**O que ajustei:** pedi pra ela ser mais específica, tipo "lista as 4 principais técnicas de prompt que aparecem nas fontes, explica cada uma em poucas linhas e fala de qual documento tirou cada info". Aí sim a resposta ficou bem mais organizada e eu conseguia ver de onde vinha cada informação.

**Outra coisa que testei:** pedi pra ela "agir como um professor" explicando um exemplo prático. Isso mudou completamente a resposta — ficou bem mais fácil de entender do que quando eu só pedia a explicação direto.

**Um teste que deu "errado" (mas foi bom aprender):** perguntei algo que não tinha nas fontes que eu subi, tipo "quais são as desvantagens que os documentos não falam". A IA respondeu que não sabia dizer com certeza porque isso não estava nos materiais que eu tinha carregado. Achei interessante porque mostra que ela não fica inventando coisa que não tem base - só responde com o que realmente está nas fontes.

**Dificuldades que tive:**
- Quando eu perguntava algo muito aberto, a resposta vinha rasa. Tive que aprender a ser mais específico.
- Às vezes ela ficava repetindo muito de uma fonte só. Tive que pedir pra cruzar informação de fontes diferentes.
- Alguns termos em inglês não vinham traduzidos, então comecei a pedir pra responder em português e explicar o termo em inglês do lado.

---

## O que eu aprendi (resumo)

**O que é um LLM:** é o modelo por trás de IAs como o ChatGPT. Ele foi treinado lendo uma quantidade gigante de texto e aprendeu a prever qual palavra faz sentido vir depois da outra. É por isso que ele consegue "conversar" com a gente.

**O que é engenharia de prompts:** é basicamente aprender a perguntar melhor pra IA. Quanto mais clara e detalhada a pergunta, melhor a resposta.

**Técnicas que aprendi:**
- Perguntar direto, sem exemplo (isso se chama zero-shot)
- Dar um ou dois exemplos antes de pedir a tarefa, pra IA entender o padrão que eu quero (few-shot)
- Definir um "papel" pra IA assumir, tipo "aja como um professor" (isso ajuda muito a mudar o tom da resposta)
- Pedir pra ela pensar passo a passo antes de responder, principalmente em coisa mais lógica ou de cálculo

**Dicas que vou usar daqui pra frente:**
- Ser específico sobre o formato que eu quero (lista, tabela, resumo curto)
- Dar contexto suficiente sem exagerar
- Não me contentar com a primeira resposta - ir ajustando a pergunta até ficar boa

---

## Glossário rápido

- **Prompt:** a pergunta ou instrução que você manda pra IA
- **LLM:** o modelo de linguagem que roda por trás da IA
- **Token:** um pedacinho de texto (palavra ou parte dela) que a IA processa
- **Zero-shot:** pedir a tarefa direto, sem exemplo
- **Few-shot:** dar exemplos antes de pedir a tarefa
- **Chain-of-thought:** pedir pra IA explicar o raciocínio passo a passo
- **Alucinação:** quando a IA inventa uma informação errada com cara de verdade
- **NotebookLM:** ferramenta do Google onde você sobe seus próprios materiais e conversa com uma IA que só responde com base neles

---

## Prompts que quero reaproveitar depois

- "Resume os pontos principais da fonte X em tópicos"
- "Cria 5 perguntas sobre esse tema baseadas só nas fontes e me dá o gabarito"
- "Compara esses dois conceitos numa tabela"
- "Explica isso como se eu tivesse acabado de conhecer o assunto, com um exemplo prático"
- "Quais pontos ainda não ficaram claros nas fontes que eu subi?"

---

Feito como parte do desafio de projeto da DIO, usando o NotebookLM como ferramenta de estudo.
