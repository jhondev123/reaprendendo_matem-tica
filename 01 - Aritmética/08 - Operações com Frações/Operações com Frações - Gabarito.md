---
tipo: gabarito
tema: Aritmética
conceito: "[[Operações com Frações]]"
tags:
  - aritmetica
  - gabarito
---
# Operações com Frações: Gabarito

**Voltar aos exercícios:** [[Operações com Frações - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $\frac{5}{7}$
**2.** $\frac{3}{6} + \frac{2}{6} = \frac{5}{6}$
**3.** $\frac{10}{12} - \frac{9}{12} = \frac{1}{12}$
**4.** $\frac{15}{5} - \frac{2}{5} = \frac{13}{5}$
**5.** Simplificando 2 com 14 e 9 com 3: $\frac{1}{1} \cdot \frac{3}{7} = \frac{3}{7}$
**6.** $\frac{3}{4} \cdot \frac{8}{9} = \frac{24}{36} = \frac{2}{3}$
**7.** $6 \cdot \frac{4}{3} = \frac{24}{3} = 8$ (cabem 8 "três quartos" em 6 inteiros)
**8.** $\frac{4}{9}$ e $-\frac{7}{5}$

## 🟡 Médio
**1.** $\frac{3}{6} + \frac{4}{6} - \frac{5}{6} = \frac{2}{6} = \frac{1}{3}$
**2.** $\frac{1}{4} \cdot \frac{1}{2} = \frac{1}{8}$
**3.** $\frac{5}{6} \div \frac{1}{6} = \frac{5}{6} \cdot 6 = 5$
**4.** Primeiro a potência: $\left(-\frac{3}{2}\right)^2 = \frac{9}{4}$. Depois a multiplicação: $\frac{2}{3} \cdot \frac{9}{4} = \frac{18}{12} = \frac{3}{2}$. Então: $-\frac{3}{4} + \frac{1}{6} + \frac{3}{2} = -\frac{9}{12} + \frac{2}{12} + \frac{18}{12} = \frac{11}{12}$.
**5.** $-\frac{1}{8} - \frac{1}{4} \cdot 4 + \frac{4}{8} = -\frac{1}{8} - 1 + \frac{1}{2} = -\frac{1}{8} - \frac{8}{8} + \frac{4}{8} = -\frac{5}{8}$
**6.** Restaram $\frac{2}{3}$ do que havia: $\frac{2}{3} \cdot \frac{3}{5} = \frac{2}{5}$ do tanque.
**7.** (a) A: $\frac{30}{40} = \frac{3}{4}$; B: $\frac{10}{20} = \frac{1}{2}$. (b) $\frac{\frac{3}{4} + \frac{1}{2}}{2} = \frac{\frac{5}{4}}{2} = \frac{5}{8}$. (c) $\frac{30 + 10}{40 + 20} = \frac{40}{60} = \frac{2}{3}$.
São diferentes porque o lote A tem **o dobro** de exemplos e deveria "pesar" mais. A média simples dá o mesmo peso aos dois lotes. Note que $\frac{2}{3} = \frac{40 \cdot \frac{3}{4} + 20 \cdot \frac{1}{2}}{60}$ é uma **média ponderada**.
**8.** Por porção: $\frac{3}{4} \div 6 = \frac{3}{24} = \frac{1}{8}$ de xícara. Para 10 porções: $10 \cdot \frac{1}{8} = \frac{10}{8} = \frac{5}{4}$ de xícara (uma xícara e um quarto).

## 🔴 Difícil
**1.** $\frac{99}{100}$.
Cada termo se quebra numa diferença: $\frac{1}{n(n+1)} = \frac{1}{n} - \frac{1}{n+1}$. (Confira: $\frac{1}{2} - \frac{1}{3} = \frac{3 - 2}{6} = \frac{1}{6}$. ✔️)
$$\left(1 - \tfrac{1}{2}\right) + \left(\tfrac{1}{2} - \tfrac{1}{3}\right) + \left(\tfrac{1}{3} - \tfrac{1}{4}\right) + \dots + \left(\tfrac{1}{99} - \tfrac{1}{100}\right)$$
Os termos do meio se cancelam aos pares (por isso a soma se chama **telescópica**) e sobra $1 - \frac{1}{100} = \frac{99}{100}$.

**2.** $\frac{1}{2026}$.
Cada fator é $1 - \frac{1}{n} = \frac{n-1}{n}$: $\;\frac{1}{2} \cdot \frac{2}{3} \cdot \frac{3}{4} \cdots \frac{2025}{2026}$. Cada numerador cancela o denominador anterior, e sobra $\frac{1}{2026}$.

**3.** $\frac{8}{5}$.
De baixo para cima: $1 + \frac{1}{2} = \frac{3}{2}$; $\;\frac{1}{3/2} = \frac{2}{3}$; $\;1 + \frac{2}{3} = \frac{5}{3}$; $\;\frac{1}{5/3} = \frac{3}{5}$; $\;1 + \frac{3}{5} = \frac{8}{5}$.

**4.** **R\$ 60.000.**
Depois do primeiro irmão, restam $\frac{2}{3}$ da herança. O segundo leva $\frac{1}{4}$ disso, então sobram $\frac{3}{4} \cdot \frac{2}{3} = \frac{1}{2}$ da herança para o terceiro. Se metade vale R\$ 30.000, a herança era de R\$ 60.000.
Conferindo: o primeiro recebeu 20.000; restaram 40.000; o segundo recebeu 10.000; restaram 30.000. ✔️
💡 *Ideia-chave: acompanhar a fração que **sobra** é mais fácil do que acompanhar a que se gasta.*

## 💻 Extra em C#
**1.** Um esboço:
```csharp
public static Fracao operator +(Fracao a, Fracao b)
    => new Fracao(a.Num * b.Den + b.Num * a.Den, a.Den * b.Den).Simplificar();

public static Fracao operator *(Fracao a, Fracao b)
    => new Fracao(a.Num * b.Num, a.Den * b.Den).Simplificar();

public static Fracao operator /(Fracao a, Fracao b)
    => a * new Fracao(b.Den, b.Num); // multiplica pelo inverso
```
**2.** Com `Fracao`, o resultado é exatamente $\frac{99}{100}$. Com `double`, você vai ver algo como `0.9899999999999999` ou `0.99`: o arredondamento binário acumula pequenos erros a cada soma.
