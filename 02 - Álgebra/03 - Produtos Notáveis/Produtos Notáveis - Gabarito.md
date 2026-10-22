---
tipo: gabarito
tema: Álgebra
conceito: "[[Produtos Notáveis]]"
tags:
  - algebra
  - gabarito
---
# Produtos Notáveis: Gabarito

**Voltar aos exercícios:** [[Produtos Notáveis - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $x^2 + 6x + 9$
**2.** $x^2 - 10x + 25$
**3.** $a^2 - 16$
**4.** $4x^2 + 4x + 1$
**5.** $9a^2 - 12ab + 4b^2$
**6.** $x^4 - 1$
**7.** $(50 + 1)^2 = 2601$; $\;(100 - 1)(100 + 1) = 9999$
**8.** $16$ e $4$: $\;x^2 + 8x + 16 = (x + 4)^2$ (o termo do meio é $2 \cdot x \cdot 4$)

## 🟡 Médio
**1.** $\frac{x^2}{4} + \frac{x}{3} + \frac{1}{9}$
**2.** $0{,}25a^2 - 2 \cdot 0{,}5a \cdot 2 + 4 = 0{,}25a^2 - 2a + 4$
**3.** (a) $3 - 2 = 1$ (b) $5 + 2\sqrt{5} + 1 = 6 + 2\sqrt{5}$
**4.** $x^3 + 3 \cdot x^2 \cdot 2 + 3 \cdot x \cdot 4 + 8 = x^3 + 6x^2 + 12x + 8$
**5.** $4x$
**6.** $(2026 - 2025)(2026 + 2025) = 1 \cdot 4051 = 4051$
**7.** $(a + b)^2 = a^2 + 2ab + b^2 \Rightarrow 49 = a^2 + b^2 + 20 \Rightarrow a^2 + b^2 = 29$
**8.** $[(x + y) + 1]^2 = (x + y)^2 + 2(x + y) + 1 = x^2 + 2xy + y^2 + 2x + 2y + 1$

## 🔴 Difícil
**1.** **500.**
O denominador é uma diferença de quadrados: $252^2 - 248^2 = (252 - 248)(252 + 248) = 4 \cdot 500 = 2000$. Então $\frac{1.000.000}{2000} = 500$.

**2.** $x^2 + \frac{1}{x^2} = $ **7** e $x^3 + \frac{1}{x^3} = $ **18**.
Elevando ao quadrado: $\left(x + \frac{1}{x}\right)^2 = x^2 + 2 \cdot x \cdot \frac{1}{x} + \frac{1}{x^2} = x^2 + 2 + \frac{1}{x^2}$. Então $9 = x^2 + \frac{1}{x^2} + 2$, e daí $x^2 + \frac{1}{x^2} = 7$.
Para o cubo: $\left(x + \frac{1}{x}\right)^3 = x^3 + 3x + \frac{3}{x} + \frac{1}{x^3} = x^3 + \frac{1}{x^3} + 3\left(x + \frac{1}{x}\right)$. Então $27 = x^3 + \frac{1}{x^3} + 9$, e $x^3 + \frac{1}{x^3} = 18$.
💡 *Ideia-chave: o produto $x \cdot \frac{1}{x} = 1$ simplifica o termo do meio.*

**3.** Sejam $n, n+1, n+2, n+3$. Agrupe: $n(n + 3) = n^2 + 3n$ e $(n + 1)(n + 2) = n^2 + 3n + 2$. Chamando $m = n^2 + 3n$:
$$n(n+1)(n+2)(n+3) + 1 = m(m + 2) + 1 = m^2 + 2m + 1 = (m + 1)^2$$
É um quadrado perfeito: $(n^2 + 3n + 1)^2$. (Teste: $1 \cdot 2 \cdot 3 \cdot 4 + 1 = 25 = 5^2$ ✔️)

**4.** **2025.**
$2026 \cdot 2024 = (2025 + 1)(2025 - 1) = 2025^2 - 1$. Então $\sqrt{2025^2 - 1 + 1} = \sqrt{2025^2} = 2025$.

## 💻 Extra em C#
**1.** A diferença entre $(a + b)^2$ e $a^2 + 2ab + b^2$ fica abaixo de `1e-9` (só erro de arredondamento). Já $(a + b)^2 - (a^2 + b^2)$ dá exatamente $2ab$, longe de zero.
**2.**
```csharp
double DistQuadDireta(double[] a, double[] b)
    => a.Zip(b, (x, y) => (x - y) * (x - y)).Sum();

double DistQuadExpandida(double[] a, double[] b)
{
    double aa = a.Sum(x => x * x);
    double bb = b.Sum(x => x * x);
    double ab = a.Zip(b, (x, y) => x * y).Sum();
    return aa - 2 * ab + bb;
}
```
