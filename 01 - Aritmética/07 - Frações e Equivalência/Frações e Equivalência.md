---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Frações
  - Frações equivalentes
  - Simplificação de frações
  - Número misto
tags:
  - aritmetica
---
# Frações e Equivalência

> [!abstract] Em uma frase
> Uma fração $\frac{a}{b}$ é **uma divisão** ($a \div b$), e muitas frações diferentes representam **o mesmo número**: multiplicar ou dividir o numerador e o denominador pelo mesmo valor não muda a fração.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[MMC e MDC]], [[Números Inteiros]] · **Próximo:** [[Operações com Frações]]
**Praticar:** [[Frações e Equivalência - Exercícios]] · [[Frações e Equivalência - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Interpretar uma fração como **parte de um todo**, como **divisão** e como **operador** ("3/4 de…").
- Gerar frações equivalentes e **simplificar até a forma irredutível**.
- Converter entre **fração imprópria** e **número misto**.
- **Comparar e ordenar** frações e localizá-las na reta.

---

## 1. Os vários sentidos de uma fração

$$\frac{3}{4} \quad \begin{array}{l} \leftarrow \text{numerador: quantas partes eu pego} \\[4pt] \leftarrow \text{denominador: em quantas partes o todo foi dividido} \end{array}$$

| Sentido | Exemplo |
|---|---|
| **Parte de um todo** | comi 3 de 4 pedaços da pizza |
| **Divisão** | $\frac{3}{4} = 3 \div 4 = 0{,}75$ (3 pizzas divididas entre 4 pessoas) |
| **Operador** | $\frac{3}{4}$ **de** 20 $= 20 \div 4 \cdot 3 = 15$ |
| **Número na reta** | $\frac{3}{4}$ fica entre 0 e 1, a três quartos do caminho |
| **Razão** | 3 acertos para cada 4 tentativas (mais em [[Razão, Proporção e Regra de Três]]) |

> [!important] A fração é uma divisão
> Por isso **o denominador nunca pode ser zero** (lembre de [[Operações Fundamentais#7. Por que não se divide por zero|por que não se divide por zero]]).
> E o sinal pode ficar em qualquer lugar: $-\frac{3}{4} = \frac{-3}{4} = \frac{3}{-4}$.

## 2. Tipos de fração

- **Própria:** numerador menor que o denominador, ou seja, menor que 1: $\frac{3}{5}$
- **Imprópria:** numerador maior ou igual ao denominador, ou seja, maior ou igual a 1: $\frac{7}{3}$
- **Aparente:** é um inteiro disfarçado: $\frac{12}{4} = 3$

**Número misto:** $\frac{7}{3} = 2\frac{1}{3}$ ("dois inteiros e um terço"), porque $7 = 3 \cdot 2 + 1$ (quociente **2**, resto **1**).
De volta: $2\frac{1}{3} = \frac{2 \cdot 3 + 1}{3} = \frac{7}{3}$.

> [!warning] Na álgebra, evite o número misto
> $2\frac{1}{3}$ pode ser confundido com $2 \cdot \frac{1}{3}$. Daqui em diante, prefira a fração imprópria $\frac{7}{3}$.

## 3. Frações equivalentes

$$\frac{2}{3} = \frac{4}{6} = \frac{6}{9} = \frac{20}{30}$$

São o **mesmo número** (a mesma quantidade de pizza, cortada em mais pedaços).

> [!tip] Por que funciona
> Multiplicar o numerador e o denominador por 5 é multiplicar a fração por $\frac{5}{5} = 1$:
> $$\frac{2}{3} \cdot \frac{5}{5} = \frac{10}{15}$$
> E multiplicar por 1 não muda nada ([[Operações Fundamentais#3. Propriedades|elemento neutro]]).

**Simplificar** é o caminho de volta: dividir o numerador e o denominador por um fator comum. A fração é **irredutível** quando $\text{mdc}(\text{num}, \text{den}) = 1$.

- Aos poucos: $\frac{36}{48} = \frac{18}{24} = \frac{9}{12} = \frac{3}{4}$
- De uma vez, pelo [[MMC e MDC|MDC]]: $\text{mdc}(36, 48) = 12 \Rightarrow \frac{36 \div 12}{48 \div 12} = \frac{3}{4}$
- Pela fatoração, "cortando" os fatores comuns: $\frac{2^3 \cdot 3^2 \cdot 5}{2^2 \cdot 3^3} = \frac{2 \cdot 5}{3} = \frac{10}{3}$

## 4. Comparando frações

| Situação | Regra | Exemplo |
|---|---|---|
| Mesmo denominador | maior numerador → maior fração | $\frac{5}{7} > \frac{3}{7}$ |
| Mesmo numerador | **menor** denominador → maior fração (pedaços maiores) | $\frac{4}{9} > \frac{4}{11}$ |
| Casos gerais | reduza ao **mesmo denominador** (o MMC) | $\frac{2}{3}$ vs $\frac{5}{8}$: $\frac{16}{24} > \frac{15}{24}$ |
| Atalho (frações positivas) | **multiplicação cruzada**: $\frac{a}{b}$ vs $\frac{c}{d}$ → compare $a \cdot d$ com $b \cdot c$ | $\frac{2}{3}$ vs $\frac{5}{8}$: $16 > 15$ |

## 5. Frações na reta

Para marcar $\frac{7}{4}$: divida cada unidade em **4** partes e conte **7** delas a partir do zero. Fica entre 1 e 2, porque $\frac{7}{4} = 1\frac{3}{4}$.

```
0         1         2
|--+--+--+|--+--+--+|
              ^ 7/4
```

Negativas ficam à esquerda: $-\frac{5}{3} = -1\frac{2}{3}$ fica entre $-2$ e $-1$.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: operador
> $\frac{2}{5}$ de 40: $40 \div 5 = 8$ (um quinto) e $8 \cdot 2 = 16$.

> [!example] Exemplo 2: encontrar o termo que falta
> $\frac{3}{8} = \frac{x}{56}$. De 8 para 56, o denominador foi multiplicado por 7; então $x = 3 \cdot 7 = 21$.

> [!example] Exemplo 3: ordenar
> Ordene $\frac{2}{3}, \frac{3}{5}, \frac{5}{8}$. O MMC de 3, 5 e 8 é 120: $\frac{80}{120}, \frac{72}{120}, \frac{75}{120}$. Ordem crescente: $\frac{3}{5} < \frac{5}{8} < \frac{2}{3}$.

> [!example] Exemplo 4: simplificar uma expressão
> $\frac{(-2)^3 \cdot 9}{-12 \cdot 6} = \frac{-72}{-72} = 1$. Ou, cortando antes: $\frac{-8 \cdot 9}{-12 \cdot 6} = \frac{8 \cdot 9}{12 \cdot 6} = \frac{2 \cdot 3}{3 \cdot 2} = 1$.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $\frac{2 + 3}{2 + 5} = \frac{3}{5}$ ("cortei o 2") | $\frac{5}{7}$ | só se cortam **fatores** (multiplicações), **nunca parcelas** (somas) |
| $\frac{1}{8} > \frac{1}{6}$ porque $8 > 6$ | $\frac{1}{8} < \frac{1}{6}$ | mais pedaços significa pedaços menores |
| $\frac{6}{0} = 0$ | não existe | o denominador não pode ser zero |
| $\frac{0}{6}$ "não existe" | $= 0$ | |
| Simplificar só o numerador | dividir **os dois** pelo mesmo número | senão a fração muda |

> [!danger] O erro nº 1 da álgebra começa aqui
> "Cortar" termos de uma soma, como em $\frac{x + 3}{x} = 3$, é o erro mais comum de toda a matemática escolar. Grave: **só se corta o que está multiplicando o numerador inteiro e o denominador inteiro.** Isso volta com força em [[Frações Algébricas]].

---

## 💻 Conexão com programação e ML

- Em C#, `3 / 4` dá **0** (divisão inteira!). Use `3.0 / 4`, `3 / 4.0` ou `(double)a / b`. Já `decimal` é mais preciso para dinheiro.
- Para guardar frações sem perder precisão, uma `record struct Fracao(long Num, long Den)` com simplificação pelo MDC funciona bem (veja o extra dos exercícios).
- **Em ML**, praticamente toda métrica é uma fração: **acurácia** $= \frac{\text{acertos}}{\text{total}}$, **precisão** $= \frac{VP}{VP + FP}$, **recall** $= \frac{VP}{VP + FN}$. E **probabilidade** é uma fração entre 0 e 1 ([[Probabilidade Básica]]).

---

## 🔗 Conexões
- **Usa:** [[Operações Fundamentais]] (a fração é uma divisão), [[MMC e MDC]] (simplificar e comparar), [[Múltiplos, Divisores e Primos]] (cortar fatores).
- **É usado em:** [[Operações com Frações]], [[Números Decimais]] (toda fração vira decimal), [[Razão, Proporção e Regra de Três]], [[Porcentagem]] ($\frac{x}{100}$), [[Conjuntos Numéricos]] (os racionais $\mathbb{Q}$).
- **Na álgebra:** [[Frações Algébricas]] e as equações com frações ([[Equações do 1º Grau]]).
- **Mais adiante:** [[Probabilidade Básica]] e o coeficiente angular de uma reta, que é uma fração ([[Equação da Reta]]).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Cite três significados da fração $\frac{3}{4}$.
2. Por que multiplicar o numerador e o denominador pelo mesmo número não altera a fração?
3. Como saber se uma fração é irredutível? Simplifique $\frac{45}{60}$ de uma vez.
4. Converta $\frac{23}{6}$ em número misto. Que operação você usou?
5. Como comparar $\frac{5}{9}$ e $\frac{4}{7}$ rapidamente?
6. Por que $\frac{2+3}{2+5} \neq \frac{3}{5}$? Qual é a regra sobre o que se pode "cortar"?
