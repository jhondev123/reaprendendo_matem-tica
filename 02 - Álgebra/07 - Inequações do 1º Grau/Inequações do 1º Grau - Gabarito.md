---
tipo: gabarito
tema: Álgebra
conceito: "[[Inequações do 1º Grau]]"
tags:
  - algebra
  - gabarito
---
# Inequações do 1º Grau: Gabarito

**Voltar aos exercícios:** [[Inequações do 1º Grau - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $x > 4$ → $]4, +\infty[$
**2.** $x \leq 5$ → $]-\infty, 5]$
**3.** $x < -4$ → $]-\infty, -4[$ (dividiu por $-3$: inverteu)
**4.** $3 \geq x$, ou seja, $x \leq 3$ → $]-\infty, 3]$
**5.** $2x < 8 \Rightarrow x < 4$ → $]-\infty, 4[$
**6.** (a) $]2, +\infty[$ (b) $[-1, 3[$ (c) $]-\infty, 0]$
**7.** $-1, 0, 1, 2, 3$
**8.** **Falso.** Por exemplo, $1 < 2$, mas $-1 > -2$.

## 🟡 Médio
**1.** $\times 6$: $3x - 6 > 2x \Rightarrow x > 6$ → $]6, +\infty[$
**2.** $\times 12$: $3(x - 1) - 4(2x + 1) \leq 12 \Rightarrow 3x - 3 - 8x - 4 \leq 12 \Rightarrow -5x \leq 19 \Rightarrow x \geq -\frac{19}{5}$ → $\left[-\frac{19}{5}, +\infty\right[$
**3.** $-4 < 2x \leq 4 \Rightarrow -2 < x \leq 2$ → $]-2, 2]$
**4.** $x > 2$ e $x \leq 6$ → $]2, 6]$
**5.** $\times 10$: $2x - 15 \geq 5x + 3 \Rightarrow -3x \geq 18 \Rightarrow x \leq -6$ → $]-\infty, -6]$
**6.** $\frac{x}{3} - \frac{1}{2} < 2 \Rightarrow \frac{x}{3} < \frac{5}{2} \Rightarrow x < \frac{15}{2}$ → $\left]-\infty, \frac{15}{2}\right[$
**7.** $1 - \sqrt{2} < 0$, então dividir por ele **inverte**: $x < 1$ → $]-\infty, 1[$
**8.** $50 + 0{,}1m < 30 + 0{,}2m \Rightarrow m > 200$. **Acima de 200 minutos.**
**9.** $2x \geq 3 \Rightarrow x \geq 1{,}5$

## 🔴 Difícil
**1.** **4.**
Multiplicando tudo por 12: $4 < n < 9$. Os inteiros são 5, 6, 7 e 8.

**2.** **$k > 1$.**
A solução é $x = \frac{5 + k}{2}$. Queremos $\frac{5 + k}{2} > 3 \Rightarrow 5 + k > 6 \Rightarrow k > 1$.

**3.** **Nota 8.**
$\frac{6{,}5 + 8 + 5{,}5 + x}{4} \geq 7 \Rightarrow 20 + x \geq 28 \Rightarrow x \geq 8$.

**4.** **11 inteiros.**
É um sistema de duas inequações:
- $3x - 7 < 2x + 1 \Rightarrow x < 8$
- $2x + 1 < 4x + 9 \Rightarrow -8 < 2x \Rightarrow x > -4$

Então $-4 < x < 8$, e os inteiros são $-3, -2, \dots, 7$: são $7 - (-3) + 1 = 11$.

## 💻 Extra em C#
**1.** O menor $x$ positivo (com passo 0,1) é **1,5**, o mesmo valor da inequação $2x - 3 \geq 0$. (Cuidado: somando 0,1 repetidamente com `double`, o valor pode ficar em `1.4999999999999998` e "pular" o 1,5. Prefira gerar os valores como `i / 10.0`.)
**2.**
```csharp
double Limitar(double v, double min, double max)
    => v < min ? min : (v > max ? max : v);
```
