---
tipo: gabarito
tema: Álgebra
conceito: "[[Equações do 2º Grau]]"
tags:
  - algebra
  - gabarito
---
# Equações do 2º Grau: Gabarito

**Voltar aos exercícios:** [[Equações do 2º Grau - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** (a) $a = 3$, $b = -5$, $c = 2$ (b) $a = 1$, $b = 0$, $c = -9$ (c) $a = -1$, $b = 4$, $c = 0$
**2.** $x = \pm 5$
**3.** $x(x - 7) = 0 \Rightarrow x = 0$ ou $x = 7$
**4.** $x^2 = 9 \Rightarrow x = \pm 3$
**5.** $x^2 = -4$: **sem raiz real**
**6.** Soma 5 e produto 6: $x = 2$ ou $x = 3$
**7.** Soma $-1$ e produto $-12$: $x = 3$ ou $x = -4$
**8.** (a) $\Delta = 16 - 16 = 0$: uma raiz (b) $\Delta = 1 - 4 = -3$: nenhuma (c) $\Delta = 9 + 16 = 25$: duas

## 🟡 Médio
**1.** $\Delta = 25$; $x = \frac{3 \pm 5}{4}$: $x = 2$ ou $x = -\frac{1}{2}$
**2.** $(x - 3)^2 = 0 \Rightarrow x = 3$ (raiz dupla)
**3.** $\Delta = 4 + 12 = 16$; $x = \frac{-2 \pm 4}{6}$: $x = \frac{1}{3}$ ou $x = -1$
**4.** $(x + 3)^2 = 16 \Rightarrow x + 3 = \pm 4$: $x = 1$ ou $x = -7$
**5.** $\Delta = 4 + 4 = 8$, e $\sqrt{8} = 2\sqrt{2}$. Então $x = \frac{2 \pm 2\sqrt{2}}{2} = 1 \pm \sqrt{2}$
**6.** $\times 6$: $3x^2 - 2x - 1 = 0$, com $\Delta = 16$: $x = 1$ ou $x = -\frac{1}{3}$
**7.** $\times 2$: $x^2 - 3x + 2 = 0 \Rightarrow (x - 1)(x - 2) = 0$: $x = 1$ ou $x = 2$
**8.** $(x - \sqrt{3})^2 = 0 \Rightarrow x = \sqrt{3}$ (raiz dupla)
**9.** Soma $\sqrt{2} + 1$ e produto $\sqrt{2}$: as raízes são $1$ e $\sqrt{2}$ (confira: $1 + \sqrt{2}$ ✔️ e $1 \cdot \sqrt{2}$ ✔️)
**10.** $x(x + 1) = 132 \Rightarrow x^2 + x - 132 = 0 \Rightarrow (x + 12)(x - 11) = 0$. Como os números são positivos: **11 e 12**.
**11.** $x(x + 4) = 60 \Rightarrow (x + 10)(x - 6) = 0$. Como a medida é positiva, $x = 6$: **6 m por 10 m**.
**12.** Soma $= -\frac{-8}{2} = 4$; produto $= \frac{3}{2}$.

## 🔴 Difícil
**1.** **$k < 4$.**
Duas raízes reais distintas exigem $\Delta > 0$: $16 - 4k > 0 \Rightarrow k < 4$.

**2.** $x_1^2 + x_2^2 = $ **19** e $\frac{1}{x_1} + \frac{1}{x_2} = $ **5/3**.
Soma $S = 5$ e produto $P = 3$.
- $x_1^2 + x_2^2 = (x_1 + x_2)^2 - 2x_1x_2 = 25 - 6 = 19$ (é o [[Produtos Notáveis|quadrado da soma]] ao contrário).
- $\frac{1}{x_1} + \frac{1}{x_2} = \frac{x_1 + x_2}{x_1x_2} = \frac{5}{3}$.

💡 *Ideia-chave: escrever o que se pede em função da soma e do produto.*

**3.** $x^2 - 4x + 1 = 0$.
Soma: $(2 + \sqrt{3}) + (2 - \sqrt{3}) = 4$. Produto: $(2 + \sqrt{3})(2 - \sqrt{3}) = 4 - 3 = 1$. Uma equação com essa soma e esse produto é $x^2 - Sx + P = 0$.

**4.** **6 amigos.**
Com $n$ amigos, cada um pagaria $\frac{240}{n}$; com $n - 2$, pagaram $\frac{240}{n - 2}$. Então
$$\frac{240}{n - 2} - \frac{240}{n} = 20$$
Multiplicando por $n(n - 2)$: $240n - 240(n - 2) = 20n(n - 2) \Rightarrow 480 = 20n^2 - 40n \Rightarrow n^2 - 2n - 24 = 0 \Rightarrow (n - 6)(n + 4) = 0$.
Como $n > 0$, $n = 6$. (Verificação: 240 ÷ 6 = 40 e 240 ÷ 4 = 60, ou seja, R\$ 20 a mais ✔️)

## 💻 Extra em C#
**1.**
```csharp
double[] Bhaskara(double a, double b, double c)
{
    if (a == 0) throw new ArgumentException("Não é do 2º grau");
    double delta = b * b - 4 * a * c;
    if (delta < 0) return Array.Empty<double>();
    if (delta == 0) return new[] { -b / (2 * a) };
    double r = Math.Sqrt(delta);
    return new[] { (-b + r) / (2 * a), (-b - r) / (2 * a) };
}
```
**2.** A raiz pequena sai muito imprecisa (às vezes até `0`), porque $-b + \sqrt{\Delta}$ subtrai dois números quase iguais (cerca de $10^8$ cada). A correção calcula primeiro a raiz "grande", que não tem esse problema, e depois a pequena pelo produto:
```csharp
double q = -0.5 * (b + Math.Sign(b) * Math.Sqrt(delta));
double x1 = q / a;   // raiz grande, estável
double x2 = c / q;   // raiz pequena, via x1 · x2 = c/a
```
