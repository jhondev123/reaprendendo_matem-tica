---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Números negativos
  - Regra de sinais
  - Módulo
  - Valor absoluto
tags:
  - aritmetica
---
# Números Inteiros

> [!abstract] Em uma frase
> Os inteiros acrescentam os **negativos** aos naturais. Somar e subtrair é **andar na reta**; multiplicar e dividir segue a **regra de sinais**.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Operações Fundamentais]] · **Próximo:** [[Expressões Numéricas]]
**Praticar:** [[Números Inteiros - Exercícios]] · [[Números Inteiros - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Localizar inteiros na reta, comparar e achar **oposto** e **módulo**.
- Somar e subtrair inteiros sem decorar regra, pensando em **saldo** ou na **reta**.
- Aplicar a **regra de sinais** na multiplicação e na divisão, e entender por que $(-)\cdot(-) = (+)$.
- Diferenciar $(-2)^2$ de $-2^2$.

---

## 1. A reta numérica

```
  ←──┼────┼────┼────┼────┼────┼────┼────┼────┼──→
    -4   -3   -2   -1    0   +1   +2   +3   +4
```

$$\mathbb{Z} = \{\dots, -3, -2, -1, 0, 1, 2, 3, \dots\}$$

- **Mais à direita é maior.** Por isso $-2 > -5$: dever 2 é melhor do que dever 5.
- **Oposto (ou simétrico):** o mesmo número do outro lado do zero. O oposto de $3$ é $-3$; o de $-7$ é $7$. A soma de um número com o seu oposto dá $0$.
- **Módulo (valor absoluto):** a **distância até o zero**, que nunca é negativa. $\lvert -5 \rvert = 5$ e $\lvert 5 \rvert = 5$.

## 2. Adição e subtração: pense em dinheiro

Positivo é **crédito**; negativo é **dívida**.

| Conta | Pensamento | Resultado |
|---|---|---|
| $5 + (-3)$ | tenho 5, devo 3 | $2$ |
| $-5 + 3$ | devo 5, tenho 3 | $-2$ |
| $-5 + (-3)$ | devo 5 e devo mais 3 | $-8$ |
| $-3 - 5$ | devo 3 e gasto mais 5 | $-8$ |

> [!important] Subtrair é somar o oposto
> $$a - b = a + (-b)$$
> Então $-3 - (-5) = -3 + 5 = 2$. "Tirar uma dívida de 5" é o mesmo que ganhar 5.

**Regra prática da soma:**
- Sinais **iguais**: some os módulos e mantenha o sinal: $-4 + (-6) = -10$.
- Sinais **diferentes**: subtraia os módulos e fique com o sinal do **maior módulo**: $-9 + 4 = -5$.

**Jogo de sinais antes de parênteses:** $+(+) = +$, $\;+(-) = -$, $\;-(+) = -$, $\;-(-) = +$.

## 3. Multiplicação e divisão: regra de sinais

| | |
|---|---|
| Sinais **iguais** | resultado **positivo**: $(-3)\cdot(-4) = 12$, $\;(-20) \div (-5) = 4$ |
| Sinais **diferentes** | resultado **negativo**: $(-3) \cdot 4 = -12$, $\;20 \div (-5) = -4$ |

> [!question]- Por que "menos com menos dá mais"? (clique para abrir)
> Observe o padrão: a cada linha, o segundo fator diminui 1 e o resultado **aumenta 2**.
> $$\begin{aligned} -2 \cdot 2 &= -4 \\ -2 \cdot 1 &= -2 \\ -2 \cdot 0 &= 0 \\ -2 \cdot (-1) &= \;?\; \to 2 \\ -2 \cdot (-2) &= \;?\; \to 4 \end{aligned}$$
> Para o padrão (e a [[Operações Fundamentais|propriedade distributiva]]) continuar valendo, $(-2)\cdot(-1)$ **tem** que dar $+2$. Não é uma regra arbitrária: é a única que mantém a matemática consistente.

**Muitos fatores:** conte os negativos. Se a quantidade for **par**, o resultado é positivo; se for **ímpar**, é negativo.
$(-1)\cdot(-2)\cdot(-3) = -6$ (são 3 negativos).

## 4. Cuidado com potências

$$(-2)^2 = (-2)\cdot(-2) = 4 \qquad \text{mas} \qquad -2^2 = -(2 \cdot 2) = -4$$

Sem parênteses, o expoente vale **só para o 2**; o sinal de menos fica de fora. Isso volta em [[Potenciação]] e em [[Expressões Numéricas]].

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1
> $-7 + 12 - 9 + 3$. Junte os positivos ($12 + 3 = 15$) e os negativos ($-7 - 9 = -16$): $15 - 16 = -1$.

> [!example] Exemplo 2
> $-8 - (-3) + (-2) = -8 + 3 - 2 = -7$

> [!example] Exemplo 3
> $\dfrac{(-6)\cdot(-5)}{-3} = \dfrac{30}{-3} = -10$

> [!example] Exemplo 4: temperatura
> De manhã fazia $-4\,°C$ e à tarde, $9\,°C$. Qual foi a variação?
> Variação = final − inicial $= 9 - (-4) = 13\,°C$.

> [!example] Exemplo 5
> $(-1)^{7} = -1$ (expoente ímpar) e $(-1)^{10} = 1$ (expoente par).

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $-3 - 5 = 2$ ou $= -2$ | $-8$ | devo 3 e devo mais 5 |
| $-3 + (-5) = +8$ | $-8$ | "menos com menos dá mais" vale **só na multiplicação e na divisão** |
| $-2^2 = 4$ | $-4$ | o expoente não "pega" o sinal sem parênteses |
| $-5 > -2$ | $-5 < -2$ | mais à esquerda na reta é menor |
| $\lvert -3 \rvert = -3$ | $3$ | distância não é negativa |

---

## 💻 Conexão com programação e ML

- `Math.Abs(-5) == 5`. Curiosidade: `Math.Abs(int.MinValue)` lança `OverflowException`, porque o `int` vai de $-2^{31}$ a $2^{31}-1$ e o oposto do mínimo não cabe.
- **O `%` do C# com negativos:** `-7 % 3 == -1`, mas o resto matemático (o da [[Operações Fundamentais#6. Divisão com resto|relação fundamental]]) é **2**, pois $-7 = 3 \cdot (-3) + 2$. Para um resto sempre positivo: `((a % n) + n) % n`.
- **Em ML:**
  - O **erro** de uma previsão (previsto − real) pode ser negativo. Por isso as métricas usam o **módulo** (MAE: erro absoluto médio) ou o **quadrado** (MSE).
  - A função de ativação **ReLU** é $\max(0, x)$: zera os negativos.
  - O **sinal** do gradiente diz para que lado ajustar cada peso. Você vai ver isso em [[Gradiente Descendente]].

---

## 🔗 Conexões
- **Usa:** [[Operações Fundamentais]] (as propriedades continuam valendo).
- **É usado em:** [[Expressões Numéricas]], [[Potenciação]] (base negativa), [[Conjuntos Numéricos]] (o conjunto $\mathbb{Z}$).
- **Na álgebra:** [[Linguagem Algébrica]] (termos com sinal), [[Equações do 1º Grau]] e [[Inequações do 1º Grau]] (multiplicar por negativo **inverte** a desigualdade).
- **Mais adiante:** [[Plano Cartesiano]] (eixos negativos), [[Função Modular]] e [[Distância entre Pontos]] (o módulo é uma distância).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. O que é o módulo de um número? Por que ele nunca é negativo?
2. Explique com a ideia de dinheiro por que $-3 - 5 = -8$.
3. Por que subtrair um número é o mesmo que somar o seu oposto? Calcule $4 - (-6)$.
4. Use o padrão das multiplicações para justificar que $(-3)\cdot(-1) = 3$.
5. Qual é o sinal de um produto com 7 fatores negativos? E com 8?
6. Qual é a diferença entre $(-3)^2$ e $-3^2$?
