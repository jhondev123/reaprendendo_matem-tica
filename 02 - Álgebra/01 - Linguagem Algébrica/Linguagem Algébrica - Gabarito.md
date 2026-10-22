---
tipo: gabarito
tema: Álgebra
conceito: "[[Linguagem Algébrica]]"
tags:
  - algebra
  - gabarito
---
# Linguagem Algébrica: Gabarito

**Voltar aos exercícios:** [[Linguagem Algébrica - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** (a) $2x$ (b) $\frac{x}{2}$ (c) $x^2 - 3$ (d) $(x - 3)^2$ (e) $3(x + 5)$ (f) $3x + 5$
**2.** (a) o dobro de um número, mais 1 (b) a média de dois números (c) a soma dos quadrados de dois números (d) o quadrado da soma de dois números
**3.** $3 \cdot 4 - 5 = 7$; $\;3 \cdot (-2) - 5 = -11$; $\;3 \cdot \frac{1}{3} - 5 = -4$
**4.** $(-3)^2 - 2 \cdot (-3) = 9 + 6 = 15$
**5.** (a) coeficiente $-5$, parte literal $x^2y$ (b) $1$ e $x$ (c) $-\frac{1}{3}$ e $ab$ (d) é um termo independente (coeficiente 7, sem parte literal)
**6.** $1{,}8 \cdot 25 + 32 = 77\,°F$; $\;1{,}8 \cdot (-10) + 32 = -18 + 32 = 14\,°F$
**7.** $x + (x + 3) + x + (x + 3) = 4x + 6$. Para $x = 2{,}5$: $10 + 6 = 16$.
**8.** (a) $n$, $n + 1$, $n + 2$ (b) $2n$ (c) $2n + 1$ (d) $2n$ e $2n + 2$

## 🟡 Médio
**1.** $a^2 = \left(-\frac{1}{2}\right)^2 = \frac{1}{4}$, e $b = 0{,}25 = \frac{1}{4}$. Numerador: $\frac{1}{4} - \frac{1}{4} = 0$. Denominador: $-\frac{1}{2} + \frac{1}{4} = -\frac{1}{4}$. Resultado: $0 \div \left(-\frac{1}{4}\right) = 0$.
**2.** Para $x = 0{,}5$: $2 \cdot 0{,}25 - 1{,}5 + 1 = 0$. Para $x = \sqrt{2}$: $2 \cdot 2 - 3\sqrt{2} + 1 = 5 - 3\sqrt{2}$.
**3.** $P = 5{,}50 + 2{,}80k$. Para 12 km: $5{,}50 + 33{,}60 = $ R\$ 39,10.
**4.** $P = 0{,}85p - 10$. Para $p = 200$: $170 - 10 = $ R\$ 160.
**5.** $n + (n + 1) + (n + 2) = 3n + 3 = 3(n + 1)$, que é 3 vezes um inteiro, ou seja, um múltiplo de 3.
**6.** $x + (2x - 4) + 20 = 3x + 16$
**7.** $\hat{y}(10) = 8 + 1{,}5 = 9{,}5$; $\;\hat{y}(-2{,}5) = -2 + 1{,}5 = -0{,}5$. Erro: $9{,}5 - 9 = 0{,}5$.

## 🔴 Difícil
**1.** Chamando o número de $x$:
$$x \to x + 5 \to 2(x + 5) = 2x + 10 \to 2x + 10 - 4 = 2x + 6 \to \frac{2x + 6}{2} = x + 3 \to x + 3 - x = 3$$
O $x$ "some" no final, então o resultado é 3 para **qualquer** número.

**2.** $(2a + 1)(2b + 1) = 4ab + 2a + 2b + 1 = 2(2ab + a + b) + 1$. É "2 vezes um inteiro, mais 1", ou seja, um ímpar.

**3.** Com algarismos $a$ (dezena) e $b$ (unidade): $(10a + b) + (10b + a) = 11a + 11b = 11(a + b)$, que é múltiplo de 11. (No exemplo, $47 + 74 = 121 = 11 \cdot 11$.)

**4.** **$3n + 1$ palitos; para 100 quadrados, 301.**
O primeiro quadrado usa 4 palitos. Cada quadrado novo aproveita um lado e precisa de **3** palitos a mais. Então $4 + 3(n - 1) = 3n + 1$. Conferindo: $n = 1$ dá 4 ✔️ e $n = 2$ dá 7 ✔️. Para $n = 100$: $301$.
💡 *Ideia-chave: achar o padrão em casos pequenos, escrever a regra com letras e conferir nos casos conhecidos.*

## 💻 Extra em C#
**1.**
```csharp
Func<double, double> f = x => 2 * x * x - 3 * x + 1;
Console.WriteLine(f(-2));            // 15
Console.WriteLine(f(0.5));           // 0
Console.WriteLine(f(Math.Sqrt(2)));  // ≈ 0,7574 (= 5 − 3√2)
```
**2.** Imprime `4`: em C#, o `=` **atribui** (calcula a direita e guarda na esquerda). Em matemática, $x = x + 1$ afirma que um número é igual a ele mesmo mais 1. Subtraindo $x$ dos dois lados, ficaria $0 = 1$, que é falso. Então não existe solução.
