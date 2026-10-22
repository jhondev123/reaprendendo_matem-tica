---
tipo: gabarito
tema: Álgebra
conceito: "[[Equações Redutíveis ao 2º Grau]]"
tags:
  - algebra
  - gabarito
---
# Equações Redutíveis ao 2º Grau: Gabarito

**Voltar aos exercícios:** [[Equações Redutíveis ao 2º Grau - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $y = 1$ ou $y = 4$ → $\{-2, -1, 1, 2\}$
**2.** $y^2 = 16$ com $y = x^2 \geq 0$ → $y = 4$ → $\{-2, 2\}$
**3.** $x(x - 2)(x + 2) = 0$ → $\{-2, 0, 2\}$
**4.** $x = 2$ ou $x^2 = 9$ → $\{-3, 2, 3\}$
**5.** ($x \neq 0$) $x^2 - 5x + 6 = 0$ → $\{2, 3\}$
**6.** $x = 9$
**7.** $x + 1 = 16 \Rightarrow x = 15$ (verificação: $\sqrt{16} = 4$ ✔️)
**8.** **Não**: $\sqrt{-1 + 2} = \sqrt{1} = 1$, mas o lado direito vale $-1$.

## 🟡 Médio
**1.** $y^2 - 10y + 9 = 0 \Rightarrow y = 1$ ou $y = 9$ → $\{-3, -1, 1, 3\}$
**2.** $y = 1$ ou $y = -4$ (descartado) → $\{-1, 1\}$
**3.** $y = x - 1$: $y = 2$ ou $y = 3$ → $\{3, 4\}$
**4.** $x + 2 = x^2 \Rightarrow x^2 - x - 2 = 0 \Rightarrow x = 2$ ou $x = -1$. Verificação: $x = 2$ dá $\sqrt{4} = 2$ ✔️; $x = -1$ dá $1 \neq -1$ ❌. Solução: $\{2\}$.
**5.** $\{4\}$ (resolvido na teoria; o $-1$ é raiz estranha)
**6.** $\left\{-\frac{1}{2}, 2\right\}$ (resolvido na teoria)
**7.** $x^2\left(x^2 - \frac{1}{4}\right) = 0$ → $\left\{-\frac{1}{2}, 0, \frac{1}{2}\right\}$
**8.** $x^2 - 4x = 0 \Rightarrow x = 0$ ou $x = 4$. O $0$ é estranho ($\sqrt{1} = 1 \neq -1$). Solução: $\{4\}$.
**9.** $0{,}\overline{1} \cdot 9 = 1$, então $x^2 - 2 = \pm 1$ → $\{-\sqrt{3}, -1, 1, \sqrt{3}\}$

## 🔴 Difícil
**1.** **$x = 9$.**
Isole uma raiz: $\sqrt{x + 7} = 7 - \sqrt{x}$. Elevando: $x + 7 = 49 - 14\sqrt{x} + x \Rightarrow 14\sqrt{x} = 42 \Rightarrow \sqrt{x} = 3 \Rightarrow x = 9$. Verificação: $\sqrt{16} + \sqrt{9} = 4 + 3 = 7$ ✔️

**2.** $\{-3, -2, 1, 2\}$.
Com $y = x^2 + x$: $y^2 - 8y + 12 = 0 \Rightarrow y = 2$ ou $y = 6$.
- $x^2 + x - 2 = 0 \Rightarrow (x + 2)(x - 1) = 0$ → $x = -2$ ou $x = 1$
- $x^2 + x - 6 = 0 \Rightarrow (x + 3)(x - 2) = 0$ → $x = -3$ ou $x = 2$

**3.** $\left\{\frac{1}{2}, 2\right\}$.
Multiplicando por $2x$ (com $x \neq 0$): $2x^2 + 2 = 5x \Rightarrow 2x^2 - 5x + 2 = 0 \Rightarrow x = \frac{5 \pm 3}{4}$, ou seja, $x = 2$ ou $x = \frac{1}{2}$.
💡 *Repare que as raízes são inversas uma da outra. Faz sentido: a equação não muda se trocarmos $x$ por $\frac{1}{x}$.*

**4.** $\{8, 27\}$.
Com $y = x^{1/3}$: $y^2 - 5y + 6 = 0 \Rightarrow y = 2$ ou $y = 3$, então $x = 8$ ou $x = 27$. Verificação: $8^{2/3} - 5 \cdot 8^{1/3} + 6 = 4 - 10 + 6 = 0$ ✔️ e $27^{2/3} - 5 \cdot 27^{1/3} + 6 = 9 - 15 + 6 = 0$ ✔️

## 💻 Extra em C#
**1.**
```csharp
double[] Biquadrada(double a, double b, double c)
    => Bhaskara(a, b, c)
        .Where(y => y >= 0)                       // x² = y precisa de y ≥ 0
        .SelectMany(y => y == 0 ? new[] { 0.0 }
                                : new[] { Math.Sqrt(y), -Math.Sqrt(y) })
        .ToArray();
```
**2.**
```csharp
var candidatos = Bhaskara(1, -3, -4);             // de x + 5 = (x − 1)²
var solucoes = candidatos
    .Where(x => Math.Abs(Math.Sqrt(x + 5) - (x - 1)) < 1e-9)
    .ToArray();                                   // só sobra o 4
```
