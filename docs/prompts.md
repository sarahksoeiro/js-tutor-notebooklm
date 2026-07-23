#  Engenharia de Prompts

## Contexto

Durante os primeiros testes com o NotebookLM, percebi que, apesar das respostas estarem tecnicamente corretas, elas não eram adequadas para um estudante iniciante em JavaScript. O modelo utilizava muitos termos técnicos, assumia conhecimentos prévios e frequentemente introduzia conceitos mais avançados sem explicar os fundamentos necessários.

Por esse motivo, decidi refinar o prompt inicial até transformar o NotebookLM em um tutor personalizado para iniciantes.

---

##  Iteração 1 — Linguagem muito técnica

###  Objetivo

Entender conceitos de JavaScript.

###  Prompt utilizado

```text
Explique o que é o DOM.
```

###  Resultado

A resposta apresentava conceitos corretos, porém utilizava termos técnicos e introduzia outros assuntos que ainda não haviam sido estudados.

###  Situação observada

As explicações eram difíceis de acompanhar para quem está começando.

###  Ajuste realizado

Passei a orientar o modelo para utilizar uma linguagem simples, acessível e com analogias do cotidiano.

---

##  Iteração 2 — Falta de conexão com os fundamentos

###  Situação observada

Ao explicar novos assuntos, como DOM, o NotebookLM não retomava conceitos básicos, como variáveis, funções ou tipos de dados, tornando a aprendizagem fragmentada.

###  Ajuste realizado

Incluí uma instrução para que todas as respostas fizessem conexões com os fundamentos do JavaScript antes de apresentar novos conceitos.

###  Resultado

As explicações passaram a seguir uma sequência mais lógica e facilitaram a compreensão dos conteúdos.

---

##  Iteração 3 — Pouca prática

###  Situação observada

As respostas eram informativas, mas não incentivavam o estudante a praticar imediatamente.

###  Ajuste realizado

Solicitei que todas as respostas terminassem com um pequeno desafio ou pergunta de fixação.

###  Resultado

O NotebookLM passou a estimular o aprendizado ativo, incentivando a aplicação imediata do conteúdo estudado.

---

#  Prompt Final

Após as melhorias, o NotebookLM passou a atuar como o **JS Tutor**, um professor virtual desenvolvido para ensinar JavaScript a iniciantes.

As principais características definidas foram:

- Linguagem simples e acessível;
- Explicações utilizando analogias;
- Revisão constante dos fundamentos;
- Progressão gradual do conteúdo;
- Exemplos de código comentados;
- Pequenos desafios ao final de cada explicação.

#  Prompt de Configuração

<details>
<summary>Clique para visualizar o prompt completo</summary>

```Você é o "JS Tutor", um professor virtual especialista, paciente e extremamente didático, focado em ensinar JavaScript para pessoas que estão dando os primeiros passos na programação.
Seu objetivo é guiar o estudante do zero ao nível intermediário, garantindo que a base conceitual esteja sempre sólida.

   Princípios Fundamentais de Atuação
Linguagem Simplificada e Acessível:
Explique conceitos complexos usando analogias do dia a dia.
Evite jargões técnicos excessivos sem antes explicá-los.
Mantenha um tom encorajador, amigável e focado na prática.
Reforço Constante da Base (Revisão Contínua):
Sempre que introduzir ou responder sobre um conceito, faça pontes com os fundamentos básicos do JavaScript (como variáveis, tipos de dados, funções e estruturas condicionais).
Relembre periodicamente a sintaxe essencial e a utilidade de elementos/comandos fundamentais, destacando para que servem na prática.
Progressão Pedagógica Gradual:
Organize o conhecimento sempre do mais simples para o mais complexo.
Se o aluno fizer uma pergunta avançada, responda de forma simplificada e direta, mas ajude-o a conectar essa dúvida avançada com os passos mais fáceis que ele precisa dominar primeiro.
Metodologia de Resposta:
O que é: Definição simples do conceito.
Para que serve: Aplicação prática no mundo real.
Exemplo de código: Um trecho pequeno, limpo e extremamente comentado.
Check de compreensão: Termine com um incentivo ou uma pequena pergunta/desafio fácil para o aluno testar o que acabou de aprender.
</details>
```
---

# 💡 Aprendizados

Durante os testes, percebi que a qualidade das respostas não dependia apenas da pergunta feita, mas principalmente do contexto fornecido ao modelo.

Definir claramente o público-alvo, a metodologia de ensino e o formato esperado das respostas tornou o NotebookLM muito mais consistente e adequado para iniciantes.

Além disso, ficou evidente que pequenos ajustes no prompt podem alterar significativamente a qualidade da experiência de aprendizagem, reforçando a importância da engenharia de prompts como etapa essencial no desenvolvimento de assistentes baseados em IA.
