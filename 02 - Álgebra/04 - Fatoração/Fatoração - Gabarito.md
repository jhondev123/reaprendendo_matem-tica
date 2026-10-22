---
tipo: gabarito
tema: Álgebra
conceito: "[[Fatoração]]"
tags:
  - algebra
  - gabarito
---
# Fatoração: Gabarito

**Voltar aos exercícios:** [[Fatoração - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $3x(2x + 3)$
**2.** $5a^2b(2a - 3b)$
**3.** $(x + 7)(x - 7)$
**4.** $(2x + 5)(2x - 5)$
**5.** $(x + 5)^2$
**6.** $(3y - 2)^2$
**7.** $(x + 3)(x + 4)$
**8.** $(x + y)(a + 3)$

## 🟡 Médio
**1.** $(x - 4)(x + 3)$
**2.** $2x(x^2 - 4) = 2x(x + 2)(x - 2)$
**3.** $(x^2 + 1)(x + 1)(x - 1)$
**4.** $3(x - 1)^2$
**5.** $(x + 2)(x^2 + 3)$
**6.** $\left(\frac{x}{2} + \frac{1}{3}\right)\left(\frac{x}{2} - \frac{1}{3}\right)$
**7.** $(0{,}1a + 0{,}7)(0{,}1a - 0{,}7)$, ou, colocando $0{,}01$ em evidência, $0{,}01(a + 7)(a - 7)$
**8.** $37 \cdot 43 = 40^2 - 3^2 = 1591$; $\;87^2 - 13^2 = 100 \cdot 74 = 7400$
**9.** Produto $-15$ e soma $-2$: $-5$ e $3$. Então $(x - 5)(x + 3)$.

## 🔴 Difícil
**1.** $a^4 + 4 = (a^2 + 2a + 2)(a^2 - 2a + 2)$.
$a^4 + 4 = a^4 + 4a^2 + 4 - 4a^2 = (a^2 + 2)^2 - (2a)^2$, uma diferença de quadrados $= (a^2 + 2 + 2a)(a^2 + 2 - 2a)$.
Para $n > 1$, o menor fator vale $n^2 - 2n + 2 = (n - 1)^2 + 1 \geq 2$, e o maior também é maior que 1. Então $n^4 + 4$ é o produto de dois números maiores que 1, logo **não é primo**. (Exemplo: $3^4 + 4 = 85 = 5 \cdot 17$, e de fato $9 - 6 + 2 = 5$ e $9 + 6 + 2 = 17$.)
💡 *Ideia-chave: "somar e subtrair a mesma coisa" para criar um padrão conhecido (a identidade de Sophie Germain).*

**2.** **2026.**
$2026^3 - 2026 = 2026(2026^2 - 1) = 2026 \cdot (2026 - 1)(2026 + 1) = 2026 \cdot 2025 \cdot 2027$. Dividindo por $2025 \cdot 2027$, sobra **2026**.

**3.** **(8, 7) e (4, 1).**
$(x - y)(x + y) = 15$, com $x + y > x - y > 0$. Os pares de fatores de 15 são $1 \cdot 15$ e $3 \cdot 5$.
- $x - y = 1$ e $x + y = 15$: somando, $2x = 16$, então $x = 8$ e $y = 7$.
- $x - y = 3$ e $x + y = 5$: então $x = 4$ e $y = 1$.

Conferindo: $64 - 49 = 15$ ✔️ e $16 - 1 = 15$ ✔️.

**4.** $n^3 - n = n(n^2 - 1) = (n - 1) \cdot n \cdot (n + 1)$, o produto de **três inteiros consecutivos**. Como você viu em [[Múltiplos, Divisores e Primos - Exercícios|Múltiplos, Divisores e Primos]], esse produto é sempre divisível por 2 e por 3, ou seja, por 6.

## 💻 Extra em C#
**1.**
```csharp
(int m, int n)? SomaEProduto(int s, int p)
{
    if (p == 0) return (0, s);
    for (int m = -Math.Abs(p); m <= Math.Abs(p); m++)
    {
        if (m == 0 || p % m != 0) continue;
        int n = p / m;
        if (m + n == s) return (m, n);
    }
    return null;
}
// SomaEProduto(7, 12)  → (3, 4)   → (x + 3)(x + 4)
// SomaEProduto(-1, -12) → (-4, 3) → (x − 4)(x + 3)
```
**2.** Devolve `null` quando **não existem inteiros** com aquela soma e aquele produto, como em $x^2 + x + 1$ ($s = 1$, $p = 1$). Isso significa que o trinômio não se fatora com números inteiros. Ele pode ter raízes irracionais ou não ter raízes reais. A ferramenta para esses casos é a fórmula de Bhaskara, em [[Equações do 2º Grau]].
