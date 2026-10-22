---
tipo: gabarito
tema: Aritmética
conceito: "[[Radiciação]]"
tags:
  - aritmetica
  - gabarito
---
# Radiciação: Gabarito

**Voltar aos exercícios:** [[Radiciação - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $9$; $3$; $-4$; $2$; $0$
**2.** $\frac{2}{3}$; $0{,}7$; $1{,}2$
**3.** $7 < \sqrt{50} < 8$ (porque $49 < 50 < 64$) e $10 < \sqrt{120} < 11$ (porque $100 < 120 < 121$).
**4.** $2\sqrt{3}$; $5\sqrt{2}$; $6\sqrt{2}$
**5.** $7\sqrt{2}$
**6.** (a) $\sqrt{36} = 6$ (b) $\sqrt{25} = 5$
**7.** (a) $5^{1/2}$ e $7^{2/3}$ (b) $8^{1/3} = 2$; $16^{3/4} = (\sqrt[4]{16})^3 = 2^3 = 8$
**8.** $\sqrt{-16}$ **não existe** nos reais (nenhum real ao quadrado dá negativo). $\sqrt[3]{-8} = -2$ **existe**, pois $(-2)^3 = -8$.

## 🟡 Médio
**1.** $2\sqrt{2} + 3\sqrt{2} - 4\sqrt{2} = \sqrt{2}$
**2.** (a) $\frac{\sqrt{2}}{2}$ (b) $\frac{6\sqrt{3}}{3} = 2\sqrt{3}$ (c) $\frac{10\sqrt{5}}{3 \cdot 5} = \frac{10\sqrt{5}}{15} = \frac{2\sqrt{5}}{3}$
**3.** $0{,}5 + (-0{,}5) - 2 = -2$
**4.** $0{,}\overline{4} = \frac{4}{9}$, então $\frac{2}{3} + \frac{2}{3} = \frac{4}{3}$.
**5.** $\sqrt{8} = 2\sqrt{2}$, então $(\sqrt{2} + 2\sqrt{2})^2 = (3\sqrt{2})^2 = 9 \cdot 2 = 18$.
**6.** $27^{2/3} = (\sqrt[3]{27})^2 = 9$; $\;16^{-1/2} = \frac{1}{4}$; $\;0{,}01^{1/2} = 0{,}1 = \frac{1}{10}$. Então $9 - \frac{1}{4} + \frac{1}{10} = \frac{180 - 5 + 2}{20} = \frac{177}{20}$ $(= 8{,}85)$.
**7.** $\sqrt{72} = 6\sqrt{2}$ cm $\approx 6 \cdot 1{,}414 = 8{,}484 \approx 8{,}48$ cm.
**8.** $\sqrt{25} - 3 - 4 = 5 - 7 = -2$; $\;-2 \cdot \frac{1}{2} = -1$.

## 🔴 Difícil
**1.** $2 + \sqrt{3}$.
Queremos $(a + \sqrt{3})^2 = a^2 + 2a\sqrt{3} + 3 = (a^2 + 3) + 2a\sqrt{3}$. Comparando com $7 + 4\sqrt{3}$: $2a = 4$, então $a = 2$, e de fato $a^2 + 3 = 7$ ✔️. Logo $\sqrt{7 + 4\sqrt{3}} = 2 + \sqrt{3}$.
(Esse $(a + b)^2 = a^2 + 2ab + b^2$ é um [[Produtos Notáveis|produto notável]].)

**2.** $\sqrt{5} + \sqrt{7}$ é maior.
Os dois são positivos, então podemos comparar os quadrados:
- $(\sqrt{5} + \sqrt{7})^2 = 5 + 2\sqrt{35} + 7 = 12 + 2\sqrt{35}$
- $(\sqrt{3} + \sqrt{9})^2 = 3 + 2\sqrt{27} + 9 = 12 + 2\sqrt{27}$

Como $\sqrt{35} > \sqrt{27}$, o primeiro é maior.
💡 *Ideia-chave: elevar ao quadrado para "sumir" com as raízes (só vale porque os números são positivos).*

**3.** **10.**
$4^2 = 16 < 20 < 25 = 5^2$, então $4 < \sqrt{20} < 5$. E $14^2 = 196 < 200 < 225 = 15^2$, então $14 < \sqrt{200} < 15$. Os inteiros entre eles vão de 5 a 14: são **10**.

**4.** **9.**
Racionalizando cada termo com o conjugado:
$$\frac{1}{\sqrt{k} + \sqrt{k+1}} = \frac{\sqrt{k+1} - \sqrt{k}}{(\sqrt{k+1} + \sqrt{k})(\sqrt{k+1} - \sqrt{k})} = \frac{\sqrt{k+1} - \sqrt{k}}{(k+1) - k} = \sqrt{k+1} - \sqrt{k}$$
A soma vira $(\sqrt{2} - \sqrt{1}) + (\sqrt{3} - \sqrt{2}) + \dots + (\sqrt{100} - \sqrt{99})$. É telescópica, como a de [[Operações com Frações]]: sobra $\sqrt{100} - \sqrt{1} = 10 - 1 = 9$.

## 💻 Extra em C#
**1.**
```csharp
double RaizBabilonica(double a)
{
    double x = a, anterior;
    int iteracoes = 0;
    do
    {
        anterior = x;
        x = (x + a / x) / 2;
        iteracoes++;
    } while (Math.Abs(x - anterior) >= 1e-12);
    Console.WriteLine($"{iteracoes} iterações");
    return x;
}
```
Para $a = 2$, a partir de $x = 2$, são cerca de 6 iterações: 1,5 → 1,41667 → 1,4142157 → 1,41421356… A quantidade de casas corretas praticamente **dobra** a cada passo.
**2.** `NaN` (não há raiz real de −1); `NaN` (o `Math.Pow` com base negativa e expoente não inteiro não é definido nos reais); `-2` (`Math.Cbrt` foi feito para lidar com índice ímpar).
