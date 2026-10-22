---
tipo: gabarito
tema: Aritmética
conceito: "[[Expressões Numéricas]]"
tags:
  - aritmetica
  - gabarito
---
# Expressões Numéricas: Gabarito

**Voltar aos exercícios:** [[Expressões Numéricas - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $2 + 12 = 14$
**2.** $6 \cdot 2 = 12$
**3.** $30 - 3 + 1 = 28$
**4.** $5 \cdot 4 = 20$
**5.** $25 - 3 \cdot 8 = 25 - 24 = 1$
**6.** $\frac{20}{5} = 4$
**7.** $-(-1) = 1$ (ou, trocando os sinais: $-6 + 9 - 2 = 1$)
**8.** $7 - 2 \cdot 3 = 7 - 6 = 1$

## 🟡 Médio
**1.** $(3 + 4) \cdot 2 = 14$ → $15 - 14 = 1$ → $2 \cdot 1 + 6 = 8$ → $40 - 8 = $ **32**.
**2.** $-9 + (-8) - (-1) = -9 - 8 + 1 = $ **−16**.
**3.** Numerador: $16 - 12 = 4$. Denominador: $4$. Então $\frac{4}{4} + (-5) = 1 - 5 = $ **−4**.
**4.** $\sqrt{100} - 6 - 8 = 10 - 14 = $ **−4**. (Repare: $\sqrt{36 + 64} \neq \sqrt{36} + \sqrt{64}$.)
**5.** $[-12 + (-9)] \div (-7) = (-21) \div (-7) = $ **3**.
**6.** Ele fez a subtração antes da multiplicação. O certo é $20 - 12 + 2 = $ **10**.
**7.** `(a + b) / (2 * c)`. Com os valores: $\frac{6 + 10}{2 \cdot 2} = \frac{16}{4} = 4$.
⚠️ `(a + b) / 2 * c` estaria **errado**: daria $\frac{16}{2} \cdot 2 = 16$.

## 🔴 Difícil
**1.** **Maior: 19**, com $(2 + 3) \cdot 4 - 1$. **Menor: 11**, com $2 + 3 \cdot (4 - 1)$.
Todas as opções: sem parênteses dá $13$; $(2 + 3) \cdot 4 - 1 = 19$; $2 + 3 \cdot (4 - 1) = 11$; $(2 + 3) \cdot (4 - 1) = 15$; $2 + (3 \cdot 4 - 1) = 13$.
💡 *Para crescer, a multiplicação precisa "pegar" o maior número possível.*

**2.** **4.** De dentro para fora: $6 - 7 = -1$; $5 - (-1) = 6$; $4 - 6 = -2$; $3 - (-2) = 5$; $2 - 5 = -3$; $1 - (-3) = 4$.

**3.** $3 \oplus 5 = 2 \cdot 3 - 5 = 1$, então $1 \otimes (-2) = 1 \cdot (-2) + 1 = $ **−1**.
$5 \otimes (-2) = -10 + 1 = -9$, então $3 \oplus (-9) = 6 - (-9) = $ **15**.
Os resultados são diferentes porque essas operações não são associativas.

**4.** Uma solução possível para cada um (há outras):
- $0 = 44 - 44$
- $1 = 44 \div 44$
- $2 = 4 \div 4 + 4 \div 4$
- $3 = (4 + 4 + 4) \div 4$
- $4 = (4 - 4) \cdot 4 + 4$
- $5 = (4 \cdot 4 + 4) \div 4$

## 💻 Extra em C#
```
14     // 2 + 12
16     // (8 / 2) * 4
1      // XOR: 010 ^ 011 = 001
8      // Math.Pow devolve double
6      // 7 / 2 == 3 (divisão inteira!), 3 * 2 == 6
7      // 7.0 / 2 == 3.5, 3.5 * 2 == 7
```
As duas últimas linhas mostram que **o tipo** (`int` ou `double`) muda o resultado da divisão.
