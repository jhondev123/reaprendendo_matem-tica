---
tipo: gabarito
tema: Aritmética
conceito: "[[Números Decimais]]"
tags:
  - aritmetica
  - gabarito
---
# Números Decimais: Gabarito

**Voltar aos exercícios:** [[Números Decimais - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** (a) $\frac{3}{4}$ (b) $\frac{1}{8}$ (c) $\frac{12}{5}$
**2.** (a) $0{,}375$ (b) $0{,}35$ (c) $1{,}25$
**3.** (a) $4{,}18$ (b) $3{,}77$
**4.** (a) $0{,}06$ (b) $0{,}06$ ($15 \cdot 4 = 60$, com 3 casas: $0{,}060$)
**5.** (a) $120 \div 4 = 30$ (b) $75 \div 25 = 3$
**6.** $0{,}405 < 0{,}45 < 0{,}5 < 0{,}54$
**7.** (a) $3{,}14$ (b) $7{,}90$
**8.** Finitos: $\frac{3}{40}$ ($40 = 2^3 \cdot 5$) e $\frac{7}{25}$ ($25 = 5^2$). Dízimas: $\frac{5}{12}$ (tem o fator 3) e $\frac{2}{15}$ (tem o fator 3).

## 🟡 Médio
**1.** (a) $\frac{7}{9}$ (b) $\frac{27}{99} = \frac{3}{11}$ (c) $1 + \frac{3}{9} = \frac{4}{3}$
**2.** (a) $\frac{16 - 1}{90} = \frac{15}{90} = \frac{1}{6}$ (b) $2 + \frac{45}{990} = 2 + \frac{1}{22} = \frac{45}{22}$
**3.** $\frac{1}{3} + \frac{1}{6} - \frac{1}{2} = \frac{2 + 1 - 3}{6} = 0$
**4.** $0{,}\overline{9} = 1$, então: $(0{,}2 + 0{,}2) \cdot (1 + 1{,}5) \div 0{,}5 = 0{,}4 \cdot 2{,}5 \div 0{,}5 = 1 \div 0{,}5 = 2$
**5.** $0{,}5 + 0{,}3 - 0{,}3 = 0{,}5$
**6.** $0{,}\overline{6} = \frac{2}{3}$. Numerador: $\frac{2}{3} - \frac{1}{2} = \frac{1}{6}$. Dividindo por $0{,}25 = \frac{1}{4}$: $\frac{1}{6} \cdot 4 = \frac{2}{3}$. E $(-0{,}5)^2 = 0{,}25 = \frac{1}{4}$. Total: $\frac{2}{3} + \frac{1}{4} = \frac{8 + 3}{12} = \frac{11}{12}$.
**7.** $6{,}29 \cdot 42{,}5 = 267{,}325 \approx$ **R\$ 267,33**
**8.** (1) Pela fração geratriz: $0{,}\overline{9} = \frac{9}{9} = 1$. (2) Pelo método: $x = 0{,}999\dots$, $10x = 9{,}999\dots$, então $9x = 9$ e $x = 1$. (Também vale: $3 \cdot \frac{1}{3} = 3 \cdot 0{,}333\dots = 0{,}999\dots$, e $3 \cdot \frac{1}{3} = 1$.)

## 🔴 Difícil
**1.** **8.**
O período tem 6 algarismos (142857). Como $2026 = 6 \cdot 337 + 4$, depois de 337 períodos completos o 2026º algarismo é o **4º** do período: 1, 4, 2, **8**.
💡 *É a [[Operações Fundamentais#6. Divisão com resto|divisão com resto]] de novo, como nos problemas de dias da semana.*

**2.** $\frac{1}{9}$.
A soma é $0{,}1111\dots = 0{,}\overline{1} = \frac{1}{9}$. (Você vai ver isso como série geométrica em [[Séries Geométricas Infinitas]]: $\frac{0{,}1}{1 - 0{,}1} = \frac{1}{9}$.)

**3.** **15 frações.**
O decimal é finito quando o denominador (já irredutível) tem só os fatores 2 e 5. Entre 2 e 10, servem $b \in \{2, 4, 5, 8, 10\}$. Contando os numeradores $a < b$ sem fator comum com $b$:
- $b = 2$: 1 → **1**
- $b = 4$: 1, 3 → **2**
- $b = 5$: 1, 2, 3, 4 → **4**
- $b = 8$: 1, 3, 5, 7 → **4**
- $b = 10$: 1, 3, 7, 9 → **4**

Total: $1 + 2 + 4 + 4 + 4 = 15$.

**4.** **1.**
Com $x = 0{,}\overline{ab}$, temos $100x = ab{,}\overline{ab}$, e subtraindo: $99x = ab$, ou seja, $x = \frac{ab}{99}$.
Então $0{,}\overline{12} + 0{,}\overline{87} = \frac{12}{99} + \frac{87}{99} = \frac{99}{99} = 1$.

## 💻 Extra em C#
**1.**
```
False                  // double é binário: 0.1 e 0.2 são aproximados
0.30000000000000004
True                   // decimal trabalha em base 10
2                      // arredondamento bancário: o empate vai para o par
3                      // o arredondamento "da escola"
```
**2.**
```csharp
bool QuaseIgual(double a, double b, double tolerancia = 1e-9)
    => Math.Abs(a - b) < tolerancia;
```
