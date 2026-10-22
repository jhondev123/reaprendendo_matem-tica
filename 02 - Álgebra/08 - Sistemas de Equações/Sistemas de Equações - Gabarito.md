---
tipo: gabarito
tema: Álgebra
conceito: "[[Sistemas de Equações]]"
tags:
  - algebra
  - gabarito
---
# Sistemas de Equações: Gabarito

**Voltar aos exercícios:** [[Sistemas de Equações - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** **Sim**: $2 + 3 = 5$ ✔️ e $4 - 3 = 1$ ✔️.
**2.** $x = 10 - y \Rightarrow 10 - 2y = 4 \Rightarrow y = 3$, $x = 7$ → $(7, 3)$
**3.** $x + 2x = 9 \Rightarrow x = 3$, $y = 6$ → $(3, 6)$
**4.** Somando: $3x = 9 \Rightarrow x = 3$, $y = 1$ → $(3, 1)$
**5.** Subtraindo a 2ª da 1ª: $2x = 4 \Rightarrow x = 2$; então $2 + 2y = 8 \Rightarrow y = 3$ → $(2, 3)$
**6.** **Impossível (SI)**: subtraindo, $0 = 2$. São retas paralelas.
**7.** **Indeterminado (SPI)**: a 2ª é o dobro da 1ª. É a mesma reta, com infinitas soluções.
**8.** $x + y = 30$ e $x - y = 6$. Somando: $2x = 36$, então **18 e 12**.

## 🟡 Médio
**1.** $(2, 3)$ (resolvido na teoria, pela adição).
**2.** $3x + 2y = 24$ e $x = y + 3$, então $5y + 9 = 24$, ou seja, $y = 3$ e $x = 6$ → $(6, 3)$
**3.** $2x + 5y = 19$ e $x = 5 - y$, então $10 + 3y = 19$, ou seja, $y = 3$ e $x = 2$ → $(2, 3)$
**4.** $p = 13 - 2c$. Então $c + 3(13 - 2c) = 14 \Rightarrow c + 39 - 6c = 14 \Rightarrow -5c = -25 \Rightarrow c = 5$, e $p = 3$. **Café: R\$ 5; pão: R\$ 3.**
**5.** $c + m = 40$ e $4c + 2m = 130$. Multiplicando a 1ª por $-2$ e somando: $2c = 50$. **25 carros e 15 motos.**
**6.** $a + e = 17$ e $5a - 2e = 50$. Multiplicando a 1ª por 2 e somando: $7a = 84 \Rightarrow a = 12$ e $e = 5$. **12 acertos.**
**7.** Somando: $2\sqrt{2}\,x = 4 \Rightarrow x = \sqrt{2}$; então $y = 3 - 2 = 1$ → $(\sqrt{2}, 1)$
**8.** **$k = 4$.** Multiplicando a 1ª por 2: $2x + 4y = 6$. Se $k = 4$, a 2ª fica $2x + 4y = 5$: o mesmo lado esquerdo com resultados diferentes. As retas são paralelas, e o sistema é impossível. (Pela regra de Cramer: $D = 1 \cdot k - 2 \cdot 2 = k - 4 = 0$.)

## 🔴 Difícil
**1.** $(2, 3)$.
Com $u = \frac{1}{x}$ e $v = \frac{1}{y}$: $u + v = \frac{5}{6}$ e $u - v = \frac{1}{6}$. Somando: $2u = 1 \Rightarrow u = \frac{1}{2}$; então $v = \frac{1}{3}$. Logo, $x = 2$ e $y = 3$.
💡 *Ideia-chave: uma troca de variável transforma um sistema "estranho" num sistema linear.*

**2.** **Ana 6, Beto 7 e Caio 10.**
Somando as três: $2(A + B + C) = 13 + 17 + 16 = 46$, então $A + B + C = 23$. Daí $C = 23 - 13 = 10$, $A = 23 - 17 = 6$ e $B = 23 - 16 = 7$.

**3.** **47.**
Com dezena $a$ e unidade $b$: $a + b = 11$ e $(10b + a) - (10a + b) = 27 \Rightarrow 9b - 9a = 27 \Rightarrow b - a = 3$. Somando com a primeira: $2b = 14 \Rightarrow b = 7$ e $a = 4$. (Verificação: $74 - 47 = 27$ ✔️)

**4.** **10 kg do tipo A e 20 kg do tipo B.**
$a + b = 30$ e $30a + 45b = 40 \cdot 30 = 1200$. Com $b = 30 - a$: $30a + 1350 - 45a = 1200 \Rightarrow -15a = -150 \Rightarrow a = 10$.

## 💻 Extra em C#
**1.**
```csharp
(double x, double y)? Resolver2x2(double a1, double b1, double c1,
                                  double a2, double b2, double c2)
{
    double d = a1 * b2 - a2 * b1;
    if (d == 0) return null; // retas paralelas ou coincidentes
    return ((c1 * b2 - c2 * b1) / d, (a1 * c2 - a2 * c1) / d);
}
// Resolver2x2(2, 3, 13, 3, -2, 0) → (2, 3)
```
