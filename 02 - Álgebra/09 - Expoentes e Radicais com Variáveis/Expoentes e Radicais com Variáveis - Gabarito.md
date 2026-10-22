---
tipo: gabarito
tema: Álgebra
conceito: "[[Expoentes e Radicais com Variáveis]]"
tags:
  - algebra
  - gabarito
---
# Expoentes e Radicais com Variáveis: Gabarito

**Voltar aos exercícios:** [[Expoentes e Radicais com Variáveis - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** (a) $x^8$ (b) $a^3$ (c) $y^8$
**2.** (a) $4x^6y^2$ (b) $-27a^6$
**3.** $\frac{1}{x^3}$ e $x^{-5}$
**4.** (a) $x^{1/2}$ (b) $x^{2/3}$ (c) $x^{-1/2}$
**5.** (a) $x$ (b) $x^2$
**6.** (a) $x^3$ (b) $5x$ (c) $x^3\sqrt{x}$
**7.** (a) $\frac{\sqrt{x}}{x}$ (b) $\frac{3\sqrt{3x}}{3x} = \frac{\sqrt{3x}}{x}$
**8.** (a) F (b) F (é $x^6$) (c) F (d) V

## 🟡 Médio
**1.** $x^{-4}y^2 \cdot x^3y = x^{-1}y^3 = \frac{y^3}{x}$
**2.** $3a^3b^2$
**3.** (a) $x^{5/6} = \sqrt[6]{x^5}$ (b) $\frac{x^{3/2}}{x^1} = x^{1/2} = \sqrt{x}$
**4.** $3x\sqrt{2x}$
**5.** $\sqrt{2} - 1$
**6.** $\frac{3 + \sqrt{5}}{2}$
**7.** (a) $3x - x^{-1/2}$ (b) $x^{3/2} + 2x^{1/2} + x^{-1/2}$ (c) $4x^{-3} - 2x^{-1/3}$
**8.** $8 - \frac{1}{2} + 1 = \frac{17}{2}$
**9.** $x - y$ (diferença de quadrados). Para os valores dados: $0{,}49 - 0{,}09 = 0{,}4$. (Conferindo pelas raízes: $(0{,}7 - 0{,}3)(0{,}7 + 0{,}3) = 0{,}4 \cdot 1 = 0{,}4$ ✔️)

## 🔴 Difícil
**1.** $\sqrt{3} - \sqrt{2}$.
$(\sqrt{a} - \sqrt{b})^2 = a + b - 2\sqrt{ab}$. Precisamos de $a + b = 5$ e $ab = 6$: $a = 3$, $b = 2$. Como $\sqrt{3} > \sqrt{2}$, o resultado é positivo, como uma raiz quadrada deve ser.

**2.** $\dfrac{2\sqrt{3} + 3\sqrt{2} - \sqrt{30}}{12}$.
1. Multiplique por $(\sqrt{2} + \sqrt{3}) - \sqrt{5}$. O denominador fica $(\sqrt{2} + \sqrt{3})^2 - 5 = 2 + 2\sqrt{6} + 3 - 5 = 2\sqrt{6}$.
2. Temos $\frac{\sqrt{2} + \sqrt{3} - \sqrt{5}}{2\sqrt{6}}$. Multiplique por $\frac{\sqrt{6}}{\sqrt{6}}$: $\frac{\sqrt{12} + \sqrt{18} - \sqrt{30}}{12} = \frac{2\sqrt{3} + 3\sqrt{2} - \sqrt{30}}{12}$.

**3.** $\frac{244}{27}$.
$4^x = (2^2)^x = (2^x)^2 = 9$. E $8^{-x} = (2^3)^{-x} = (2^x)^{-3} = 3^{-3} = \frac{1}{27}$. Soma: $9 + \frac{1}{27} = \frac{244}{27}$.
💡 *Ideia-chave: escrever tudo como potência de 2 e usar $(a^m)^n = (a^n)^m$.*

**4.** $\sqrt[3]{3}$ é maior.
$\sqrt{2} = 2^{1/2}$ e $\sqrt[3]{3} = 3^{1/3}$. Elevando os dois (positivos) à 6ª potência: $(2^{1/2})^6 = 2^3 = 8$ e $(3^{1/3})^6 = 3^2 = 9$. Como $9 > 8$, $\sqrt[3]{3} > \sqrt{2}$.

## 💻 Extra em C#
**1.** `Math.Pow(8, 1/3)` dá `1`, porque `1/3` é divisão inteira e vale `0`, e $8^0 = 1$. `Math.Pow(8, 1.0/3)` dá `2` (aproximadamente).
**2.** Os dois dão `0.41421356…` ✔️
