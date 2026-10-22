---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Variáveis
  - Expressões algébricas
  - Valor numérico
tags:
  - algebra
---
# Linguagem Algébrica

> [!abstract] Em uma frase
> Álgebra é aritmética com **letras no lugar de números**: a letra guarda um número que não conhecemos (ou qualquer número) e deixa escrever regras gerais de uma vez só.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Expressões Numéricas]], [[Treino Misto - Lista 4]] · **Próximo:** [[Monômios e Polinômios]]
**Praticar:** [[Linguagem Algébrica - Exercícios]] · [[Linguagem Algébrica - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Ler e escrever as **convenções** da álgebra ($3x$, $x^2$, $xy$…).
- **Traduzir** frases em português para expressões algébricas, e vice-versa.
- Calcular o **valor numérico** de uma expressão, sem errar os sinais.
- Usar letras para **provar** uma regra geral (por exemplo, "a soma de dois consecutivos é ímpar").

---

## 1. Por que usar letras?

Lembra da [[Treino Misto - Lista 4|Lista 4 do treino misto]]? "Pensei num número, multipliquei por 5, somei 0,5…". Escrever "o número pensado" toda hora cansa. Na álgebra, damos um nome a ele: $x$.

A letra pode ter três papéis:

| Papel | Exemplo | A letra é… |
|---|---|---|
| **Incógnita** (valor desconhecido) | $2x + 3 = 11$ | um número específico que queremos descobrir ($x = 4$) |
| **Variável** (qualquer valor) | $A = b \cdot h$ | qualquer número; a fórmula vale para todos |
| **Parâmetro** (valor fixo, mas genérico) | $y = ax + b$ | um número fixo, que muda de um problema para outro |

> [!tip] Se você programa, você já faz álgebra
> `double Area(double b, double h) => b * h;` é a fórmula $A = b \cdot h$. Os parâmetros do método são as variáveis da fórmula.

## 2. As convenções (a "sintaxe")

| Escrita | Significa | Observação |
|---|---|---|
| $3x$ | $3 \cdot x$ | o sinal de vezes fica implícito |
| $xy$ | $x \cdot y$ | |
| $x$ | $1 \cdot x$ | o coeficiente 1 não se escreve |
| $-x$ | $-1 \cdot x$ | |
| $x^2$ | $x \cdot x$ | lê-se "x ao quadrado" |
| $2x^2$ | $2 \cdot x \cdot x$ | o expoente vale **só para o $x$** |
| $(2x)^2$ | $2x \cdot 2x = 4x^2$ | com parênteses, vale para tudo |
| $3(x + 1)$ | $3 \cdot (x + 1)$ | |
| $\frac{x}{2}$ | $x \div 2$ | |

> [!warning] Número na frente, letra atrás
> Escrevemos $3x$, e não $x3$. E $x \cdot 3 \cdot y \cdot 2$ se simplifica para $6xy$ (os números se multiplicam entre si e as letras ficam em ordem alfabética).

## 3. Termos, coeficientes e parte literal

Em $5x^2 - 3xy + 7$:
- os **termos** (as partes separadas por $+$ ou $-$) são $5x^2$, $-3xy$ e $7$;
- em $-3xy$, o **coeficiente** é $-3$ (o número, **com o sinal**) e a **parte literal** é $xy$ (as letras com os expoentes);
- o $7$, sem letra, é o **termo independente**.

## 4. Traduzindo português ↔ álgebra

Essa é a habilidade mais importante para resolver problemas. Seja $x$ "um número":

| Português | Álgebra |
|---|---|
| o dobro de um número | $2x$ |
| a metade de um número | $\frac{x}{2}$ |
| o triplo de um número, mais 5 | $3x + 5$ |
| o triplo **da soma** de um número com 5 | $3(x + 5)$ |
| o quadrado de um número, menos 3 | $x^2 - 3$ |
| o quadrado **da diferença** entre um número e 3 | $(x - 3)^2$ |
| o inverso de um número | $\frac{1}{x}$ |
| o oposto de um número | $-x$ |
| 20% de um número | $0{,}2x$ |
| dois números consecutivos | $n$ e $n + 1$ |
| um número par / um número ímpar | $2n$ / $2n + 1$ (com $n$ inteiro) |
| a média de dois números | $\frac{a + b}{2}$ |

> [!tip] A palavra "da" pede parênteses
> "O dobro **da soma** de $x$ com 3" → $2(x + 3)$. Já "a soma do dobro de $x$ com 3" → $2x + 3$. Leia devagar: a **última** operação mencionada ("o dobro de…") é a que fica **por fora**.

> [!question]- Tente agora (clique para ver as respostas)
> Traduza: (a) a soma de um número com o seu quadrado; (b) o quadrado da soma de dois números; (c) um número menos a sua quinta parte.
> **Respostas:** (a) $x + x^2$ (b) $(a + b)^2$ (c) $x - \frac{x}{5}$

## 5. Valor numérico

É **substituir** as letras por números e resolver a [[Expressões Numéricas|expressão numérica]] que sobra.

> [!important] Regra de ouro: substitua **com parênteses**
> Calcule $x^2 - 3x$ para $x = -2$:
> $$(-2)^2 - 3 \cdot (-2) = 4 + 6 = 10$$
> Sem parênteses, você escreveria $-2^2 - 3 \cdot -2$, e erraria o sinal. **Sempre** coloque o valor entre parênteses.

> [!example] Com fração
> $2a^2 - b$ para $a = \frac{1}{2}$ e $b = -0{,}5$:
> $$2 \cdot \left(\tfrac{1}{2}\right)^2 - (-0{,}5) = 2 \cdot \tfrac{1}{4} + 0{,}5 = 0{,}5 + 0{,}5 = 1$$

> [!example] Numa fórmula
> Para converter Celsius em Fahrenheit: $F = 1{,}8C + 32$. Para $C = 25$: $F = 1{,}8 \cdot 25 + 32 = 45 + 32 = 77\,°F$.

## 6. Usando letras para provar coisas

Com números você só **testa** exemplos; com letras você **prova** para todos.

> [!example] A soma de dois números consecutivos é sempre ímpar
> Dois consecutivos: $n$ e $n + 1$. A soma é $n + (n + 1) = 2n + 1$, que tem exatamente a forma de um ímpar. ✔️ Isso vale para **qualquer** $n$, não só para os que testamos.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: tradução de problema
> "Um táxi cobra R\$ 5,50 de bandeirada e R\$ 2,80 por km rodado." Chamando os km de $k$: $P = 5{,}50 + 2{,}80k$. Para 12 km: $P = 5{,}50 + 33{,}60 = 39{,}10$.

> [!example] Exemplo 2: expressão com várias pessoas
> Ana tem $x$ anos. O irmão tem o dobro da idade dela menos 4. A mãe tem a soma das duas idades mais 20.
> Irmão: $2x - 4$. Mãe: $x + (2x - 4) + 20 = 3x + 16$.

> [!example] Exemplo 3: valor numérico com raiz
> $2x^2 - 3x + 1$ para $x = \sqrt{2}$: $\;2 \cdot (\sqrt{2})^2 - 3\sqrt{2} + 1 = 4 - 3\sqrt{2} + 1 = 5 - 3\sqrt{2}$

> [!example] Exemplo 4: truque de mágica
> "Pense num número, some 3, dobre o resultado, subtraia 6 e divida por 2. Deu o número que você pensou!"
> $x \to x + 3 \to 2(x + 3) = 2x + 6 \to 2x + 6 - 6 = 2x \to \frac{2x}{2} = x$ ✔️

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $x = -3 \Rightarrow x^2 = -9$ | $(-3)^2 = 9$ | substitua com parênteses |
| $3x$ com $x = 2$ vira $32$ | $3 \cdot 2 = 6$ | $3x$ é multiplicação |
| "triplo da soma de x com 5" $= 3x + 5$ | $3(x + 5)$ | "da soma" pede parênteses |
| $2x^2 = (2x)^2$ | $(2x)^2 = 4x^2$ | o expoente vale só para o $x$ |
| "a metade de x" $= \frac{2}{x}$ | $\frac{x}{2}$ | |

---

## 💻 Conexão com programação e ML

- ⚠️ **"=" em matemática não é "=" em C#.** Em C#, `x = x + 1` é uma **atribuição** ("pegue x, some 1 e guarde em x"). Em matemática, $x = x + 1$ é uma **afirmação** de igualdade, que é falsa para qualquer número (seria como dizer $0 = 1$). O "=" matemático é mais parecido com o `==` do C#.
- Uma expressão algébrica é uma função: `Func<double, double> f = x => 2 * x * x - 3 * x + 1;`. Calcular o valor numérico é chamar `f(-2)`.
- **Em ML**, o modelo mais simples, a regressão linear, é a expressão $\hat{y} = w \cdot x + b$. $x$ é a **variável** (o dado de entrada); $w$ e $b$ são os **parâmetros**, que o treino descobre; e $\hat{y}$ (lê-se "y chapéu") é a previsão. "Treinar" é achar os melhores valores de $w$ e $b$.

---

## 🔗 Conexões
- **Usa:** [[Expressões Numéricas]] (o valor numérico é uma expressão numérica), [[Números Inteiros]] (sinais na substituição), [[Treino Misto - Lista 4]] (a ideia de "número pensado").
- **É usado em:** [[Monômios e Polinômios]] (operar com as expressões), [[Equações do 1º Grau]] (achar o valor da incógnita) e todo o resto da álgebra.
- **Mais adiante:** [[Conceito de Função]] (uma expressão com uma variável é uma função) e [[Somatório e Produtório]] (letras com índice, como $x_1, x_2, \dots$).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Qual é a diferença entre incógnita, variável e parâmetro?
2. Qual é a diferença entre $2x^2$ e $(2x)^2$?
3. Traduza: "o dobro da diferença entre um número e 7" e "a diferença entre o dobro de um número e 7".
4. Calcule $x^2 - x$ para $x = -4$. Por que usar parênteses?
5. Como representar um número par e um número ímpar? E três números consecutivos?
6. Por que `x = x + 1` faz sentido em C#, mas não em matemática?
