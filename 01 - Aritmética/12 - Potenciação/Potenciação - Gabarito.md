---
tipo: gabarito
tema: Aritmética
conceito: "[[Potenciação]]"
tags:
  - aritmetica
  - gabarito
---
# Potenciação: Gabarito

**Voltar aos exercícios:** [[Potenciação - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $32$; $81$; $-8$; $-16$; $9$
**2.** $1$; $1$; $0$; $-1$
**3.** $\frac{8}{27}$; $0{,}04$; $\frac{1}{16}$
**4.** (a) $2^8$ (b) $5^3$ (c) $3^8$
**5.** $\frac{1}{8}$; $0{,}01$; $5^2 = 25$
**6.** (a) $4{,}5 \times 10^7$ (b) $3{,}2 \times 10^{-4}$
**7.** (a) 602.000 (b) 0,0015
**8.** (a) **V**: $8 + 8 = 16 = 2^4$ (somar duas vezes a mesma potência é multiplicar por 2) (b) **V**: potência de produto (c) **F**: $25 \neq 13$ (d) **F**: $8 \neq 9$

## 🟡 Médio
**1.** $\frac{2^3}{2^4} = 2^{-1} = \frac{1}{2}$
**2.** $-8 + 4 - 1 + \frac{1}{4} = -5 + \frac{1}{4} = -\frac{19}{4}$
**3.** $\left(\frac{3}{2}\right)^2 \cdot \frac{9}{16} - \frac{1}{4} = \frac{9}{4} \cdot \frac{9}{16} - \frac{1}{4} = \frac{81}{64} - \frac{16}{64} = \frac{65}{64}$
**4.** (a) $2^9 \cdot 2^4 = 2^{13}$ (b) $\frac{2^8}{2^5} = 2^3$ (c) $0{,}5 = 2^{-1}$, então $(2^{-1})^{-3} = 2^3$
**5.** (a) $6 \times 10^5$ (b) $2 \times 10^{8}$
**6.** $7 \times 10^9 \cdot 2 = 14 \times 10^9 = 1{,}4 \times 10^{10}$ bytes, ou cerca de **14 GB**.
**7.** $2^{30} = (2^{10})^3 = 1024^3$ e $10^9 = 1000^3$. Como $1024 > 1000$, temos $2^{30} > 10^9$.
**8.** $(0{,}01 \cdot 1000)^{-1} = 10^{-1} = 0{,}1$

## 🔴 Difícil
**1.** **9.**
Os algarismos das unidades das potências de 7 se repetem num ciclo de 4: $7^1 = 7$, $7^2 = 49$, $7^3 = 343$, $7^4 = 2401$, e depois 7, 9, 3, 1 de novo. Como $2026 = 4 \cdot 506 + 2$, o algarismo é o **2º** do ciclo: **9**.
💡 *É a [[Operações Fundamentais#6. Divisão com resto|divisão com resto]] mais uma vez.*

**2.** **12 algarismos.**
$2^{10} \cdot 5^{12} = 2^{10} \cdot 5^{10} \cdot 5^2 = 10^{10} \cdot 25 = 25$ seguido de 10 zeros, ou seja, $2 + 10 = 12$ algarismos.
💡 *Ideia-chave: formar pares $2 \cdot 5 = 10$.*

**3.** $2^{100} < 5^{50} < 3^{75}$.
Escreva todos com o mesmo expoente 25: $2^{100} = (2^4)^{25} = 16^{25}$, $\;3^{75} = (3^3)^{25} = 27^{25}$, $\;5^{50} = (5^2)^{25} = 25^{25}$. Com o mesmo expoente, basta comparar as bases: $16 < 25 < 27$.

**4.** **6.**
Coloque a menor potência em evidência: $2^{2026} + 2^{2025} = 2^{2024}(2^2 + 2^1) = 2^{2024} \cdot 6$. Dividindo por $2^{2024}$, sobra **6**.

## 💻 Extra em C#
**1.**
```csharp
long Potencia(long b, int e)
{
    long resultado = 1;
    for (int i = 0; i < e; i++) resultado *= b;
    return resultado;
}
// Potencia(2, 10) == 1024 == 1L << 10
```
**2.** Em $n = 63$. O `long` tem 64 bits, e um deles é o sinal: o maior valor é $2^{63} - 1$. Então $2^{63}$ já não cabe e "dá a volta" para um número negativo (*overflow*). Use `checked { ... }` para o C# lançar uma exceção em vez de errar em silêncio.
