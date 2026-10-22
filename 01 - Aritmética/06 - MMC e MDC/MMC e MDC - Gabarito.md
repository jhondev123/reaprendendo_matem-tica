---
tipo: gabarito
tema: Aritmética
conceito: "[[MMC e MDC]]"
tags:
  - aritmetica
  - gabarito
---
# MMC e MDC: Gabarito

**Voltar aos exercícios:** [[MMC e MDC - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** mmc = **12**, mdc = **2**.
**2.** $12 = 2^2 \cdot 3$ e $18 = 2 \cdot 3^2$. mmc = $2^2 \cdot 3^2 = 36$; mdc = $2 \cdot 3 = 6$.
**3.** $8 = 2^3$, $12 = 2^2 \cdot 3$, $20 = 2^2 \cdot 5$ → mmc = $2^3 \cdot 3 \cdot 5 = 120$.
**4.** $2^2 \cdot 3 = 12$
**5.** $252 = 198 \cdot 1 + 54$; $198 = 54 \cdot 3 + 36$; $54 = 36 \cdot 1 + 18$; $36 = 18 \cdot 2 + 0$ → **18**.
**6.** **Sim**: $15 = 3 \cdot 5$ e $28 = 2^2 \cdot 7$ não têm primos em comum. mmc = $15 \cdot 28 = 420$.
**7.** $\text{mdc}(84, 126) = 42$, então $\frac{84 \div 42}{126 \div 42} = \frac{2}{3}$.
**8.** $b = \frac{60 \cdot 4}{12} = 20$

## 🟡 Médio
**1.** É **MMC** ("juntas de novo"): $\text{mmc}(6, 8, 10) = 2^3 \cdot 3 \cdot 5 = 120$ s, ou seja, **2 minutos**.
**2.** É **MDC** ("maior número de kits iguais"): $\text{mdc}(48, 72) = 24$ kits, cada um com $48 \div 24 = 2$ brancas e $72 \div 24 = 3$ pretas.
**3.** $\text{mdc}(1920, 1080) = 120$ → **16:9**. Para a outra, $1280 = 2^8 \cdot 5$ e $1024 = 2^{10}$, então o mdc é $2^8 = 256$ → **5:4**.
**4.** É **MDC** (a maior distância que divide os dois lados): $\text{mdc}(120, 84) = 12$ m. Perímetro: $2 \cdot (120 + 84) = 408$ m. Numa cerca **fechada**, o número de estacas é igual ao número de intervalos: $408 \div 12 = $ **34 estacas**.
**5.** O número menos 7 tem que ser múltiplo de 12, 15 e 20. $\text{mmc}(12, 15, 20) = 60$, então o número é $60 + 7 = $ **67**. (Confira: $67 = 12 \cdot 5 + 7 = 15 \cdot 4 + 7 = 20 \cdot 3 + 7$.)
**6.** $72 = 2^3 \cdot 3^2$ e $96 = 2^5 \cdot 3$, então o mmc é $2^5 \cdot 3^2 = 288$ s, ou seja, **4 min 48 s**. Ana dá $288 \div 72 = 4$ voltas e Bruno, $288 \div 96 = 3$.

## 🔴 Difícil
**1.** **301.**
Se o número deixa resto 1 na divisão por 2, 3, 4, 5 e 6, então $n - 1$ é múltiplo de todos eles, ou seja, de $\text{mmc}(2,3,4,5,6) = 60$. Os candidatos são $61, 121, 181, 241, 301, \dots$ Testando a divisão por 7: $61$ (resto 5), $121$ (resto 2), $181$ (resto 6), $241$ (resto 3) e $301 = 7 \cdot 43$ ✔️.

**2.** **(12, 72), (24, 60) e (36, 48).**
Como o mdc é 12, os números são $12x$ e $12y$, com $x$ e $y$ **primos entre si** (se tivessem um fator em comum, o mdc seria maior que 12). Então $12x + 12y = 84 \Rightarrow x + y = 7$. Os pares com mdc 1 são (1, 6), (2, 5) e (3, 4). Multiplicando por 12, obtemos os três pares.
💡 *Ideia-chave: "tirar o MDC para fora" e trabalhar com números primos entre si.*

**3.** **A dá 3 voltas e B dá 2.**
A cada dente que passa, os dois avançam um dente. As marcas voltam a se encontrar quando o número de dentes que passaram for múltiplo de 24 **e** de 36: $\text{mmc}(24, 36) = 72$ dentes. Isso dá $72 \div 24 = 3$ voltas de A e $72 \div 36 = 2$ voltas de B.

**4.** **3.**
$1023 = 63 \cdot 16 + 15$; $\;63 = 15 \cdot 4 + 3$; $\;15 = 3 \cdot 5 + 0$. Então o mdc é 3.
*Curiosidade:* vale a regra $\text{mdc}(2^a - 1, 2^b - 1) = 2^{\text{mdc}(a,b)} - 1$. Aqui, $2^{\text{mdc}(10,6)} - 1 = 2^2 - 1 = 3$. ✔️

## 💻 Extra em C#
**1.**
```csharp
int Mdc(int a, int b) => b == 0 ? a : Mdc(b, a % b);
int Mmc(int a, int b) => a / Mdc(a, b) * b; // divide antes para evitar overflow
```
**2.**
```csharp
string Proporcao(int largura, int altura)
{
    int d = Mdc(largura, altura);
    return $"{largura / d}:{altura / d}";
}
```
