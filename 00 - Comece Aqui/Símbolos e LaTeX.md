---
tipo: guia
tags:
  - guia
  - notacao
---
# 🔣 Símbolos e LaTeX

Notação matemática é uma linguagem. Assim como em programação, ler bem a sintaxe é metade do caminho. Esta nota é a sua **referência rápida**: como se lê cada símbolo e como escrevê-lo no Obsidian.

## Como escrever fórmulas no Obsidian

- **Na linha do texto:** entre cifrões simples → `$x^2 + 1$` vira $x^2 + 1$
- **Em destaque, numa linha própria:** entre cifrões duplos:

```
$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$
```

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

> [!tip] Chaves agrupam
> Em LaTeX, `{ }` funciona como os parênteses de uma chamada de função: `x^{10}` gera $x^{10}$, mas `x^10` gera $x^10$ (só o 1 sobe).

## Operações e comparações

| Símbolo | Lê-se | Exemplo | LaTeX |
|---|---|---|---|
| $+$ $-$ | mais, menos | $5 - 2 = 3$ | `+` `-` |
| $\times$ $\cdot$ | vezes | $3 \cdot 4 = 12$ | `\times` `\cdot` |
| $\div$ | dividido por | $12 \div 4 = 3$ | `\div` |
| $\frac{a}{b}$ | a sobre b | $\frac{3}{4}$ | `\frac{a}{b}` |
| $\pm$ | mais ou menos | $\pm 2$ | `\pm` |
| $=$ | igual | $2 + 2 = 4$ | `=` |
| $\neq$ | diferente | $3 \neq 4$ | `\neq` |
| $\approx$ | aproximadamente | $\pi \approx 3{,}14$ | `\approx` |
| $<$ $>$ | menor que, maior que | $2 < 5$ | `<` `>` |
| $\leq$ $\geq$ | menor ou igual, maior ou igual | $x \geq 0$ | `\leq` `\geq` |

## Potências, raízes e outros

| Símbolo | Lê-se | Exemplo | LaTeX |
|---|---|---|---|
| $a^n$ | a elevado a n | $2^3 = 8$ | `a^{n}` |
| $\sqrt{a}$ | raiz quadrada de a | $\sqrt{9} = 3$ | `\sqrt{a}` |
| $\sqrt[n]{a}$ | raiz n-ésima de a | $\sqrt[3]{8} = 2$ | `\sqrt[n]{a}` |
| $\lvert x \rvert$ | módulo (valor absoluto) de x | $\lvert -5 \rvert = 5$ | `\lvert x \rvert` |
| $x_i$ | x índice i | $x_1, x_2, x_3$ | `x_{i}` |
| $\pi$ | pi | $\pi \approx 3{,}1416$ | `\pi` |
| $\Delta$ | delta (variação ou discriminante) | $\Delta = b^2 - 4ac$ | `\Delta` |
| $\infty$ | infinito | $x \to \infty$ | `\infty` |
| $n!$ | n fatorial | $4! = 24$ | `n!` |

## Somatório e produtório

| Símbolo | Lê-se | Exemplo | LaTeX |
|---|---|---|---|
| $\sum_{i=1}^{n} x_i$ | soma de x índice i, com i indo de 1 a n | $\sum_{i=1}^{3} i = 6$ | `\sum_{i=1}^{n} x_i` |
| $\prod_{i=1}^{n} x_i$ | produto de x índice i, com i indo de 1 a n | $\prod_{i=1}^{3} i = 6$ | `\prod_{i=1}^{n} x_i` |

Veja [[Somatório e Produtório]].

## Conjuntos e lógica

| Símbolo | Lê-se | Exemplo | LaTeX |
|---|---|---|---|
| $\in$ | pertence a | $3 \in \mathbb{N}$ | `\in` |
| $\notin$ | não pertence a | $-1 \notin \mathbb{N}$ | `\notin` |
| $\subset$ | está contido em | $\mathbb{N} \subset \mathbb{Z}$ | `\subset` |
| $\cup$ | união | $A \cup B$ | `\cup` |
| $\cap$ | interseção | $A \cap B$ | `\cap` |
| $\emptyset$ | conjunto vazio | $A \cap B = \emptyset$ | `\emptyset` |
| $\mathbb{N}, \mathbb{Z}, \mathbb{Q}, \mathbb{R}$ | naturais, inteiros, racionais, reais | $\sqrt{2} \in \mathbb{R}$ | `\mathbb{N}` |
| $\forall$ | para todo | $\forall x \in \mathbb{R}$ | `\forall` |
| $\exists$ | existe | $\exists x$ tal que $x^2 = 4$ | `\exists` |
| $\Rightarrow$ | implica | $x = 2 \Rightarrow x^2 = 4$ | `\Rightarrow` |
| $\Leftrightarrow$ | se e somente se | $x + 1 = 3 \Leftrightarrow x = 2$ | `\Leftrightarrow` |

Veja [[Conjuntos Numéricos]].

## Letras gregas mais usadas

| Letra | Nome | Onde aparece |
|---|---|---|
| $\alpha, \beta, \theta$ | alfa, beta, teta | ângulos; em ML, $\theta$ são os parâmetros do modelo e $\alpha$ a taxa de aprendizado |
| $\Delta, \delta$ | delta | variação, diferença |
| $\varepsilon$ | épsilon | um valor muito pequeno; erro |
| $\lambda$ | lambda | autovalores; regularização em ML |
| $\mu, \sigma$ | mi, sigma | média e desvio padrão |
| $\Sigma$ | sigma maiúsculo | somatório (e matriz de covariância) |
| $\pi$ | pi | razão entre circunferência e diâmetro; também produtório ($\Pi$) |

> [!tip] Vá completando esta nota conforme encontrar símbolos novos nos próximos temas.
