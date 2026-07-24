# JS Tutor - JavaScript para Iniciantes

> **Projeto desenvolvido para o desafio da DIO**
>
> **Tema:** JavaScript para Iniciantes  
> **Ferramenta:** NotebookLM  
> **Objetivo:** Construção de um tutor virtual utilizando Engenharia de Prompts.

> **Banner:** Substitua esta linha pela imagem do banner (`assets/banner.png`).

---

## Índice

- [Apresentação](#apresentação)
- [Objetivos](#objetivos)
- [Tema Escolhido](#tema-escolhido)
- [Curadoria de Fontes](#curadoria-de-fontes)
- [Engenharia de Prompts](#engenharia-de-prompts)
- [Prompt de Configuração](#prompt-de-configuração)
- [Guia de Estudos](#guia-de-estudos)
- [Glossário](#glossário)
- [Prompts Reutilizáveis](#prompts-reutilizáveis)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Considerações Finais](#considerações-finais)
  
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

Para construir uma base de conhecimento mais completa, o NotebookLM foi alimentado com aproximadamente **40 materiais**, incluindo documentações oficiais, artigos técnicos, materiais acadêmicos e videoaulas.

Abaixo estão algumas das principais fontes utilizadas durante o projeto:

- **JavaScript.info** — Guia completo sobre JavaScript moderno.  
  https://javascript.info/

- **W3Schools – JavaScript** — Material introdutório com exemplos práticos.  
  https://www.w3schools.com/js/

- **JavaScript: The Definitive Guide** — David Flanagan.

- **Videoaulas sobre JavaScript** (YouTube) utilizadas para complementar a abordagem prática e exemplos de código.

> **Observação:** Além das fontes listadas acima, foram utilizados diversos outros materiais, incluindo artigos especializados, conteúdos acadêmicos e aproximadamente 40 documentos e videoaulas incorporados ao NotebookLM para enriquecer sua base de conhecimento. A seleção de diferentes formatos permitiu explorar as capacidades do NotebookLM na síntese e organização de conteúdos provenientes tanto de textos quanto de vídeos.

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

Você é o "JS Tutor", um professor virtual especialista, paciente e extremamente didático, focado em ensinar JavaScript para pessoas que estão dando os primeiros passos na programação. Seu objetivo é guiar o estudante do zero ao nível intermediário, garantindo que a base conceitual esteja sempre sólida. Princípios Fundamentais de Atuação Linguagem Simplificada e Acessível: Explique conceitos complexos usando analogias do dia a dia. Evite jargões técnicos excessivos sem antes explicá-los. Mantenha um tom encorajador, amigável e focado na prática. Reforço Constante da Base (Revisão Contínua): Sempre que introduzir ou responder sobre um conceito, faça pontes com os fundamentos básicos do JavaScript (como variáveis, tipos de dados, funções e estruturas condicionais). Relembre periodicamente a sintaxe essencial e a utilidade de elementos/comandos fundamentais, destacando para que servem na prática. Progressão Pedagógica Gradual: Organize o conhecimento sempre do mais simples para o mais complexo. Se o aluno fizer uma pergunta avançada, responda de forma simplificada e direta, mas ajude-o a conectar essa dúvida avançada com os passos mais fáceis que ele precisa dominar primeiro. Metodologia de Resposta: O que é: Definição simples do conceito. Para que serve: Aplicação prática no mundo real. Exemplo de código: Um trecho pequeno, limpo e extremamente comentado. Check de compreensão: Termine com um incentivo ou uma pequena pergunta/desafio fácil para o aluno testar o que acabou de aprender.

</details>

---

## Miniguia de Estudos

Olá, futuro desenvolvedor!

Este material foi preparado para ser o seu mapa na jornada de aprendizado do JavaScript. Diferente de outras linguagens, o JavaScript é responsável por dar vida às páginas da web, permitindo que elas deixem de ser apenas conteúdos estáticos e se tornem experiências interativas.

>Este guia foi elaborado para servir como um material de apoio aos estudos de JavaScript, reunindo os principais conceitos fundamentais em uma sequência lógica e progressiva. O objetivo não é substituir a prática, mas fornecer uma base sólida para consultas rápidas, revisões e esclarecimento de dúvidas durante o aprendizado. À medida que você dominar esses conteúdos, estará preparado para explorar temas mais avançados, como Arrays, Objetos, Programação Assíncrona, Consumo de APIs, ES6+, Orientação a Objetos e frameworks modernos.

---

### Fluxo de Aprendizagem

O estudo foi organizado em uma sequência lógica, na qual cada conceito serve de base para o próximo.

Introdução
↓ 
Variáveis
↓ 
Tipos de Dados
↓
Estruturas Condicionais 
↓ 
Laços de Repetição 
↓
Funções
↓ 
DOM (Document Object Model)

---

#### Antes de começar

Para aproveitar melhor este guia, é recomendado possuir conhecimentos básicos sobre:

- **HTML:** compreender a estrutura das páginas.
- **CSS:** entender como os estilos são aplicados.
- **Lógica de programação:** conhecer a ideia de resolver problemas por meio de uma sequência de passos.

---

### 1. Introdução e Variáveis: As Caixas da Memória

#### O que é?

JavaScript é uma linguagem de programação de alto nível executada principalmente no navegador do usuário.

##### Conexão

Antes de ensinar o computador a executar ações, precisamos ensiná-lo a armazenar informações. É justamente esse o papel das variáveis.

##### Analogia

Imagine que você está organizando uma mudança. Cada variável funciona como uma caixa identificada por uma etiqueta. A etiqueta representa o nome da variável e o conteúdo armazenado representa seu valor.

#### Como declarar variáveis

##### `const`

Utilizada para valores que não serão reatribuídos.

##### `let`

Utilizada para valores que podem mudar durante a execução do programa.

##### `var`

Forma antiga de declarar variáveis. Seu uso não é recomendado devido ao comportamento relacionado ao escopo e ao hoisting.

##### Exemplo
javascript const nomeDoGato = "Frajola"; let fomeDoGato = 10; fomeDoGato = 100; // nomeDoGato = "Bolinha"; // Erro: constantes não podem ser reatribuídas.
> **Atenção**
>
> Um erro comum é tentar alterar o valor de uma constante. Sempre que o valor puder mudar, utilize `let`.

---

### 2. Tipos de Dados: O que cabe na caixa?

#### Conexão

Agora que sabemos criar variáveis, precisamos entender quais tipos de informações podem ser armazenadas nelas.

##### Analogia

Assim como uma cozinha possui recipientes apropriados para diferentes alimentos, cada tipo de dado possui uma finalidade específica.

#### Principais tipos

- **String:** textos.
- **Number:** números inteiros e decimais.
- **Boolean:** valores `true` e `false`.
- **null:** ausência intencional de valor.
- **undefined:** variável criada, mas sem valor atribuído.

##### Exemplo
javascript let preco = 25.50; let produto = "Caneta"; let temEstoque = true; console.log("5" + 2); // "52"
> **Atenção**
>
> Colocar números entre aspas faz com que eles sejam tratados como texto.

---

### 3. Estruturas Condicionais: O Cérebro do Código

#### Conexão

Depois de armazenar informações, é hora de permitir que o programa tome decisões.

##### Analogia

Pense em um GPS.

Se houver trânsito, ele escolhe outro caminho.

Caso contrário, mantém a rota original.

#### Principais estruturas

- `if`
- `else`
- `switch`

##### Exemplo
javascript let nota = 7; if (nota >= 7) { console.log("Aprovado!"); } else { console.log("Reprovado."); }
> **Atenção**
>
> Prefira utilizar `===` para comparações. O operador `==` realiza conversões automáticas que podem causar comportamentos inesperados.

---

### 4. Laços de Repetição: Automatizando Tarefas

#### Conexão

Em vez de repetir o mesmo código várias vezes, utilizamos loops para automatizar tarefas repetitivas.

##### Analogia

Imagine um atleta correndo voltas em uma pista. Ele continua repetindo o percurso até cumprir seu objetivo.

#### Principais estruturas

- `for`
- `while`
- `for...of`
- `forEach`

##### Exemplo
javascript const frutas = ["Maçã", "Banana", "Uva"]; frutas.forEach(function(fruta) { console.log("Eu gosto de " + fruta); });
> **Atenção**
>
> Um erro comum é criar um `while` cuja condição nunca deixa de ser verdadeira, gerando um loop infinito.

---

### 5. Funções: Blocos Reutilizáveis

#### Conexão

À medida que os programas crescem, repetir código deixa de ser uma boa prática. As funções permitem organizar e reutilizar tarefas.

##### Analogia

Imagine uma receita de bolo. Você escreve os passos uma única vez e pode utilizá-los sempre que quiser. As funções seguem essa mesma ideia: criar uma sequência de instruções reutilizável.

##### Exemplo
javascript function calcularMedia(n1, n2) { let resultado = (n1 + n2) / 2; return resultado; } let minhaMedia = calcularMedia(8, 10);
> **Atenção**
>
> Não confunda criar uma função com executá-la. Declarar a função apenas a torna disponível; ela só será executada quando for chamada.

---

### 6. DOM (Document Object Model): O JavaScript Encontra a Página

#### Conexão

Até aqui, o JavaScript manipulava apenas dados na memória. Com o DOM, ele passa a interagir diretamente com os elementos da página.

##### Analogia

O HTML representa a estrutura do corpo, o CSS representa sua aparência e o DOM funciona como o sistema nervoso, permitindo que o JavaScript modifique e controle os elementos da página.

#### Principais ações

- Selecionar elementos.
- Alterar textos e estilos.
- Responder a eventos do usuário.

##### Exemplo
javascript const botao = document.querySelector("#meuBotao"); botao.addEventListener("click", function () { document.body.style.backgroundColor = "blue"; });
> **Atenção**
>
> Um erro comum é tentar acessar elementos do HTML antes que eles tenham sido carregados pelo navegador.

---

## Glossário

- **API:** conjunto de funcionalidades disponibilizadas pelo navegador para o JavaScript.
- **Array:** lista ordenada de elementos.
- **Callback:** função passada como argumento para outra função.
- **Interpolação:** inserção de variáveis em textos utilizando template strings.
- **Hoisting:** comportamento em que determinadas declarações são processadas antes da execução do código.
- **Objeto:** estrutura que armazena informações em pares de chave e valor.

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
