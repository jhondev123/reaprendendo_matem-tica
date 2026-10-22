---
tipo: gabarito
tema: Aritmética
conceito: "[[Números Inteiros]]"
tags:
  - aritmetica
  - gabarito
---
# Números Inteiros: Gabarito

**Voltar aos exercícios:** [[Números Inteiros - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $-10, -7, -2, 0, 3, 5$
**2.** (a) $12$  (b) $8$  (c) $15$  (d) $3 - 3 = 0$
**3.** $-5$
**4.** $-8$
**5.** $-6 + 10 = 4$
**6.** $28$
**7.** $-9$
**8.** $(-2)^2 = 4$ e $-2^2 = -4$
**9.** $-1$ (são 5 fatores negativos, uma quantidade ímpar)
**10.** $(8 + 10) + (-15 - 3) = 18 - 18 = 0$

## 🟡 Médio
**1.** Comece de dentro para fora: $5 - 8 = -3$; depois $3 - (-3) = 6$; então $-[6] + 6 = -6 + 6 = 0$.
**2.** Numerador: $-60$. Denominador: $6$. Resultado: $-60 \div 6 = -10$.
**3.** $350 - 500 + 120 - 85 = -115$. O saldo final é **R\$ −115** (a conta está no negativo).
**4.** Variação: $14 - (-3) = 17\,°C$. Depois de cair 9: $14 - 9 = 5\,°C$.
**5.** Erros: $10 - 8 = 2$, $\;7 - 9 = -2$, $\;12 - 12 = 0$. Módulos: $2, 2, 0$. Média: $\frac{2 + 2 + 0}{3} = \frac{4}{3} \approx 1{,}33$.
Repare que a média dos erros **sem** o módulo daria $0$, como se o modelo fosse perfeito. Por isso se usa o módulo.
**6.** **Positivo.** $(-2)^{15}$ é negativo (expoente ímpar), $(-3)^8$ é positivo (expoente par) e $(-1)^3$ é negativo. Ficamos com negativo · positivo · negativo: são **dois** fatores negativos, uma quantidade par, então o produto é positivo.

## 🔴 Difícil
**1.** **−50.**
Agrupe de dois em dois: $(1 - 2) + (3 - 4) + \dots + (99 - 100)$. Cada par dá $-1$ e há 50 pares: $50 \cdot (-1) = -50$.

**2.** **0.**
Os termos alternam: $-1 + 1 - 1 + 1 \dots$ Cada par $(-1)^{\text{ímpar}} + (-1)^{\text{par}}$ dá $0$. De 1 a 2026 há 2026 termos, ou seja, 1013 pares completos. Soma: $0$.

**3.** **−120.**
Em cinco consecutivos, o do meio é a média: $-15 \div 5 = -3$. Os números são $-5, -4, -3, -2, -1$ (soma: $-15$ ✔️).
O produto tem 5 fatores negativos (quantidade ímpar), então é negativo: $5 \cdot 4 \cdot 3 \cdot 2 \cdot 1 = 120 \Rightarrow -120$.
💡 *Ideia-chave: em uma quantidade ímpar de consecutivos, o termo do meio é a soma dividida pela quantidade.*

**4.** **12 acertos.**
Ele respondeu $20 - 3 = 17$ questões. Se acertasse todas, faria $17 \cdot 5 = 85$ pontos. Cada acerto que vira erro **perde** $5 + 2 = 7$ pontos (deixa de ganhar 5 e ainda perde 2). Ele perdeu $85 - 50 = 35$ pontos, o que dá $35 \div 7 = 5$ erros. Então acertou $17 - 5 = 12$.
Conferindo: $12 \cdot 5 - 5 \cdot 2 = 60 - 10 = 50$. ✔️
💡 *Ideia-chave: começar de um caso extremo (acertou tudo) e contar quanto cada troca altera o resultado. Em [[Sistemas de Equações]], você vai resolver isso com álgebra.*

## 💻 Extra em C#
**1.**
```csharp
int Modulo(int x) => x < 0 ? -x : x;
```
**2.** O C# imprime `-1`, porque o `%` mantém o **sinal do dividendo**: $-7 = 3 \cdot (-2) + (-1)$. O resto matemático, entre $0$ e $n - 1$, é **2**: $-7 = 3 \cdot (-3) + 2$.
```csharp
int RestoMatematico(int a, int n) => ((a % n) + n) % n;
// RestoMatematico(-7, 3) == 2
```
