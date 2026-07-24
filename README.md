# JS Tutor - JavaScript para Iniciantes

> **Projeto desenvolvido para o desafio da DIO**
>
> **Tema:** JavaScript para Iniciantes  
> **Ferramenta:** NotebookLM  
> **Objetivo:** Construção de um tutor virtual utilizando Engenharia de Prompts.

> **Banner:** Substitua esta linha pela imagem do banner (`assets/banner.png`).

---

## Apresentação

Projeto desenvolvido durante o desafio da DIO utilizando o NotebookLM para criar um tutor virtual especializado em JavaScript para iniciantes.

O objetivo foi explorar o uso da Inteligência Artificial como ferramenta de aprendizagem ativa, organizando conteúdos, testando estratégias de prompts e construindo um guia de estudos reutilizável.

---

## Objetivos

- Aprender os fundamentos do JavaScript.
- Utilizar o NotebookLM como tutor personalizado.
- Desenvolver prompts eficientes.
- Criar um material de revisão para estudos futuros.

---

## Tema Escolhido

JavaScript para iniciantes.

O NotebookLM foi configurado para atuar como um professor virtual chamado **JS Tutor**, seguindo uma metodologia gradual baseada em explicações simples, exemplos práticos, analogias e revisão constante dos conceitos fundamentais.

---

## Curadoria de Fontes

As seguintes fontes foram utilizadas para compor a base de conhecimento do NotebookLM:

- https://javascript.info/
- https://www.w3schools.com/js/
- *JavaScript: The Definitive Guide* — David Flanagan

---

## Engenharia de Prompts

### Contexto

Durante os primeiros testes, percebi que o NotebookLM respondia corretamente do ponto de vista técnico, mas utilizava muitos termos avançados para um estudante iniciante.

O objetivo da engenharia de prompts foi transformar o modelo em um tutor didático, capaz de ensinar do básico ao intermediário.

### Iteração 1 — Linguagem muito técnica

**Objetivo**

Entender o conceito de DOM.

**Prompt utilizado**

```text
Explique o que é o DOM.
```

**Resultado**

A resposta utilizava termos técnicos e assumia conhecimentos prévios.

**Situação observada**

As explicações eram difíceis para iniciantes.

**Ajuste realizado**

Solicitei uma linguagem simples, com analogias e menos jargões.

---

### Iteração 2 — Falta de conexão com os fundamentos

**Situação observada**

Os novos conteúdos não retomavam conceitos fundamentais.

**Ajuste realizado**

Solicitei que cada explicação conectasse o assunto atual com variáveis, tipos de dados, funções e condicionais.

**Resultado**

O conteúdo passou a seguir uma sequência lógica.

---

### Iteração 3 — Pouca prática

**Situação observada**

As respostas eram apenas expositivas.

**Ajuste realizado**

Solicitei que todas as respostas terminassem com um pequeno desafio.

**Resultado**

O NotebookLM passou a incentivar a aprendizagem ativa.

---

### Aprendizados

A qualidade das respostas depende tanto do contexto quanto da pergunta realizada.

Definir público-alvo, metodologia e formato esperado tornou as respostas muito mais consistentes.

---

## Prompt de Configuração

Após os refinamentos, foi desenvolvido um prompt responsável por transformar o NotebookLM em um tutor especializado em JavaScript.

<details>
<summary>Clique para visualizar o prompt</summary>

Cole aqui o prompt completo do JS Tutor.

</details>

---

## Miniguia de Estudos

> Neste ponto, cole o miniguia que você produziu (Fluxo de Aprendizagem, Variáveis, Tipos de Dados, Condicionais, Loops, Funções, DOM etc.).

---

## Glossário

> Cole aqui o glossário produzido pelo NotebookLM.

---

## Prompts Reutilizáveis

```text
Explique o conceito de [CONCEITO] utilizando linguagem simples, analogias e um exemplo comentado.
```

```text
Crie três exercícios sobre [TEMA], organizados do nível básico ao intermediário.
```

```text
Meu código apresenta o erro [ERRO]. Analise o trecho abaixo, explique a causa e proponha uma solução.

[CÓDIGO]
```

```text
Como utilizar [CONCEITO] para desenvolver um(a) [TIPO DE PROJETO]? Explique passo a passo.
```

```text
Quais são as diferenças entre [CONCEITO A] e [CONCEITO B]? Apresente exemplos práticos.
```

---

## Tecnologias Utilizadas

- NotebookLM
- Markdown
- GitHub
- Inteligência Artificial Generativa

---

## Considerações Finais

Este projeto demonstra como a Engenharia de Prompts pode transformar uma ferramenta de IA em um tutor personalizado, tornando o processo de aprendizagem mais estruturado, acessível e eficiente.

Além de consolidar conhecimentos em JavaScript, o projeto reforçou a importância da curadoria de fontes, da organização do conhecimento e da elaboração de instruções claras para obtenção de melhores resultados com modelos de IA.
