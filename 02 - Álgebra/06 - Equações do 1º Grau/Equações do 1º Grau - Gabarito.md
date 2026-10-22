---
tipo: gabarito
tema: Álgebra
conceito: "[[Equações do 1º Grau]]"
tags:
  - algebra
  - gabarito
---
# Equações do 1º Grau: Gabarito

**Voltar aos exercícios:** [[Equações do 1º Grau - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $x = 8$
**2.** $x = -6$
**3.** $2x = 16 \Rightarrow x = 8$
**4.** $3x = -12 \Rightarrow x = -4$
**5.** $4x - 8 = 3x + 1 \Rightarrow x = 9$
**6.** $x = -12$
**7.** $-2x = -4 \Rightarrow x = 2$
**8.** Sim: $2 \cdot 3 - 1 = 5$ e $3 + 2 = 5$.

## 🟡 Médio
**1.** $\times 6$: $3x + 2x = 60 \Rightarrow x = 12$
**2.** $\times 12$: $4(x - 1) - 3(x + 2) = 2 \Rightarrow 4x - 4 - 3x - 6 = 2 \Rightarrow x = 12$
**3.** $2x + 6 - 3x + 3 = 5 - x \Rightarrow -x + 9 = 5 - x \Rightarrow 9 = 5$: **sem solução**.
**4.** $3x - 6 + 6 = 3x \Rightarrow 3x = 3x$: **infinitas soluções** (qualquer $x$).
**5.** (a) $C = \frac{F - 32}{1{,}8}$ (b) $t = \frac{d}{v}$ (c) $x = \frac{y - b}{w}$ (d) $h = \frac{2A}{b}$
**6.** $x + (x + 1) + (x + 2) = 84 \Rightarrow 3x + 3 = 84 \Rightarrow x = 27$. Os números são **27, 28 e 29**.
**7.** $3x + 12 = 2(x + 12) \Rightarrow x = 12$. **O filho tem 12 anos e o pai, 36.**
**8.** $0{,}85p = 170 \Rightarrow p = \frac{170}{0{,}85} = 200$. **R\$ 200.**

## 🔀 Treino misto
**1.** $\times 10$: $3x + 12 = 5x - 4 \Rightarrow 16 = 2x \Rightarrow x = 8$
**2.** $\frac{x}{3} + \frac{1}{2} = 1 \;\xrightarrow{\times 6}\; 2x + 3 = 6 \Rightarrow x = \frac{3}{2}$
**3.** $\times 10$: $4x - 1 = 5x \Rightarrow x = -1$
**4.** $\sqrt{2}\,x = 2 \Rightarrow x = \frac{2}{\sqrt{2}} = \sqrt{2}$
**5.** $\sqrt{12} = 2\sqrt{3}$, então $x\sqrt{3} = 2\sqrt{3} \Rightarrow x = 2$
**6.** $\frac{2}{3}(x - 3) = \frac{3}{2} \Rightarrow x - 3 = \frac{3}{2} \cdot \frac{3}{2} = \frac{9}{4} \Rightarrow x = \frac{21}{4}$
**7.** $x + 0{,}5 = 0{,}25 \cdot \frac{1}{2} = 0{,}125 \Rightarrow x = -0{,}375 = -\frac{3}{8}$
**8.** ($x \neq 0$) $\frac{3}{x} = \frac{3}{2} \Rightarrow x = 2$
**9.** $\sqrt{8} = 2\sqrt{2}$, então $\frac{x}{\sqrt{2}} = 3\sqrt{2} \Rightarrow x = 3\sqrt{2} \cdot \sqrt{2} = 6$
**10.** $1{,}\overline{2} - 0{,}\overline{2} = 1$ e $0{,}\overline{9} = 1$, então $1 \cdot x = 1 + 2 \Rightarrow x = 3$

## 🔴 Difícil
**1.** **15.**
$\frac{x}{3} + \frac{x}{5} + 7 = x$. Multiplicando por 15: $5x + 3x + 105 = 15x \Rightarrow 7x = 105 \Rightarrow x = 15$. (Verificação: $5 + 3 + 7 = 15$ ✔️)

**2.** **84 anos.**
$$\frac{x}{6} + \frac{x}{12} + \frac{x}{7} + 5 + \frac{x}{2} + 4 = x$$
O MMC de 6, 12, 7 e 2 é 84. Multiplicando: $14x + 7x + 12x + 420 + 42x + 336 = 84x$, ou seja, $75x + 756 = 84x$, então $9x = 756$ e $x = 84$.
(Verificação: $14 + 7 + 12 + 5 + 42 + 4 = 84$ ✔️)

**3.** **2 horas.**
Seja $t$ o tempo do segundo trem. O primeiro andou $t + 1$ horas. Eles se encontram quando percorreram a mesma distância: $60(t + 1) = 90t \Rightarrow 60 = 30t \Rightarrow t = 2$.
(Os dois estão a 180 km da estação ✔️)

**4.** **$a = 2$.**
$ax - a = 2x + 3 \Rightarrow (a - 2)x = a + 3$.
- Se $a = 2$: $0 \cdot x = 5$, que é impossível, então **não há solução**.
- Se $a \neq 2$: $x = \frac{a + 3}{a - 2}$.

💡 *Ideia-chave: o coeficiente do $x$ pode depender de um parâmetro. Quando ele zera, a equação "quebra".*

## 💻 Extra em C#
**1.**
```csharp
string Resolver(double a, double b, double c)
{
    // ax + b = c  ⇔  ax = c − b
    if (a == 0)
        return (c - b == 0) ? "infinitas soluções" : "sem solução";
    return ((c - b) / a).ToString();
}
```
**2.** Exemplo: o 🔀 1 vira $-0{,}2x + 1{,}2 = -0{,}4$ (passando tudo para a esquerda), e `Resolver(-0.2, 1.2, -0.4)` devolve `8` (ou algo como `8,000000000000002`, por causa do `double`; lembra de [[Números Decimais]]?).
