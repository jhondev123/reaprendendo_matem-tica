---
tipo: gabarito
tema: Álgebra
conceito: "[[Frações Algébricas]]"
tags:
  - algebra
  - gabarito
---
# Frações Algébricas: Gabarito

**Voltar aos exercícios:** [[Frações Algébricas - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** (a) $x \neq 2$ (b) $x \neq 3$ e $x \neq -3$ (c) $x \neq 0$ e $x \neq -4$
**2.** $\frac{2x}{3y^2}$
**3.** $\frac{3(x + 2)}{x + 2} = 3$ (com $x \neq -2$)
**4.** $x - 3$ (com $x \neq -3$)
**5.** $x + 3$ (com $x \neq -2$)
**6.** $\frac{5}{x}$
**7.** $\frac{6x}{3x^2} = \frac{2}{x}$
**8.** $\frac{4}{x} \cdot \frac{x^2}{2} = 2x$

## 🟡 Médio
**1.** $\frac{(x + 3)(x - 3)}{x(x + 3)} = \frac{x - 3}{x}$
**2.** $\frac{2x + 1}{x(x + 1)}$
**3.** $\frac{x + 3}{(x - 1)(x + 1)} = \frac{x + 3}{x^2 - 1}$
**4.** $\frac{(x + 2)(x - 2)}{(x + 2)^2} = \frac{x - 2}{x + 2}$
**5.** $\frac{(x + 1)(x - 1)}{x + 3} \cdot \frac{2(x + 3)}{x - 1} = 2(x + 1)$
**6.** $\frac{3x - 2}{6} \cdot \frac{6}{x} = \frac{3x - 2}{x}$
**7.** $\frac{0{,}5(x + 2)}{x + 2} = \frac{1}{2}$
**8.** $\frac{x(x - 3)}{(3 - x)(3 + x)} = -\frac{x}{x + 3}$ (porque $3 - x = -(x - 3)$)

## 🔴 Difícil
**1.** $\frac{x}{x + 1}$.
Numerador: $\frac{x - 1}{x}$. Denominador: $\frac{x^2 - 1}{x^2}$. Dividindo: $\frac{x - 1}{x} \cdot \frac{x^2}{(x - 1)(x + 1)} = \frac{x}{x + 1}$.

**2.** $A = \frac{1}{2}$ e $B = -\frac{1}{2}$.
Somando as frações da direita: $\frac{A(x + 1) + B(x - 1)}{x^2 - 1} = \frac{(A + B)x + (A - B)}{x^2 - 1}$. Para ser igual a $\frac{1}{x^2 - 1}$ para todo $x$: $A + B = 0$ e $A - B = 1$. Daí $A = \frac{1}{2}$ e $B = -\frac{1}{2}$.
(Isso se chama **decomposição em frações parciais** e é muito usado para calcular integrais.)

**3.** $\frac{10}{3}$.
Divida cada parcela: $\frac{a^2 + b^2}{ab} = \frac{a^2}{ab} + \frac{b^2}{ab} = \frac{a}{b} + \frac{b}{a} = 3 + \frac{1}{3} = \frac{10}{3}$.

**4.** $\frac{65535}{32768}$ (ou $2 - \frac{1}{32768}$).
Chame o produto de $P$ e multiplique por $\left(1 - \frac{1}{2}\right)$. Em cada passo aparece uma diferença de quadrados:
$$\left(1 - \tfrac{1}{2}\right)\left(1 + \tfrac{1}{2}\right) = 1 - \tfrac{1}{4} \;\to\; \left(1 - \tfrac{1}{4}\right)\left(1 + \tfrac{1}{4}\right) = 1 - \tfrac{1}{16} \;\to\; \dots \;\to\; 1 - \tfrac{1}{256^2} = 1 - \tfrac{1}{65536}$$
Então $\frac{1}{2} P = 1 - \frac{1}{65536}$, e $P = 2 - \frac{2}{65536} = 2 - \frac{1}{32768} = \frac{65535}{32768}$.
💡 *Ideia-chave: criar o primeiro fator de uma cadeia de diferenças de quadrados.*

## 💻 Extra em C#
**1.** Os resultados só diferem em $x = -3$: a primeira expressão dá `NaN` (porque $\frac{0}{0}$), e a segunda dá `-6`. A simplificação "tapa o buraco" da função original, mas a condição de existência $x \neq -3$ continua valendo.
**2.**
```csharp
double Sigmoide(double x) => 1 / (1 + Math.Exp(-x));
foreach (var x in new[] { -2.0, -0.5, 0, 1, 3 })
{
    double s = Sigmoide(x);
    double e = Math.Exp(-x);
    Console.WriteLine($"{s * (1 - s)} == {e / Math.Pow(1 + e, 2)}");
}
```
Algebricamente: $1 - \sigma = 1 - \frac{1}{1 + e^{-x}} = \frac{e^{-x}}{1 + e^{-x}}$, então $\sigma(1 - \sigma) = \frac{1}{1 + e^{-x}} \cdot \frac{e^{-x}}{1 + e^{-x}} = \frac{e^{-x}}{(1 + e^{-x})^2}$.
