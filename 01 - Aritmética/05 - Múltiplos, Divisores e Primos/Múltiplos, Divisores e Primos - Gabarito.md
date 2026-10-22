---
tipo: gabarito
tema: Aritmética
conceito: "[[Múltiplos, Divisores e Primos]]"
tags:
  - aritmetica
  - gabarito
---
# Múltiplos, Divisores e Primos: Gabarito

**Voltar aos exercícios:** [[Múltiplos, Divisores e Primos - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $7, 14, 21, 28, 35, 42$
**2.** $1, 2, 3, 4, 6, 9, 12, 18, 36$
**3.** Por 2: **sim** (termina em 6). Por 3: **sim** (soma 15). Por 4: **não** (46 não é múltiplo de 4). Por 5: **não**. Por 6: **sim** (é divisível por 2 e por 3). Por 9: **não** (15 não é múltiplo de 9).
**4.** $2, 17, 29, 41$. (Os outros: $9 = 3^2$, $21 = 3 \cdot 7$, $39 = 3 \cdot 13$, $51 = 3 \cdot 17$, $57 = 3 \cdot 19$; e o 1 não é primo.)
**5.** $84 = 2^2 \cdot 3 \cdot 7$
**6.** $360 = 2^3 \cdot 3^2 \cdot 5$
**7.** A soma é $4 + ■ + 2 = 6 + ■$, que precisa ser múltipla de 3: $■ \in \{0, 3, 6, 9\}$.
**8.** (a) V ($0 = 5 \cdot 0$)  (b) F  (c) F (6 é par e não é divisível por 4)  (d) V

## 🟡 Médio
**1.** $72 = 2^3 \cdot 3^2$, então são $(3+1)(2+1) = 12$ divisores: $1, 2, 3, 4, 6, 8, 9, 12, 18, 24, 36, 72$.
**2.** $120 = 2^3 \cdot 3 \cdot 5$. Num quadrado perfeito, **todos os expoentes são pares**. Falta um 2, um 3 e um 5: multiplicamos por $2 \cdot 3 \cdot 5 = $ **30**, obtendo $3600 = 60^2$.
**3.** $\sqrt{97} \approx 9{,}8$, então basta testar os primos 2, 3, 5 e 7. Nenhum divide 97 (é ímpar, a soma dos algarismos é 16, não termina em 0 nem 5, e $97 = 7 \cdot 13 + 6$). Logo, é primo.
**4.** **5040, 5445 e 5940.**
Por 5: $b = 0$ ou $b = 5$. Por 9: $5 + a + 4 + b = 9 + a + b$ precisa ser múltiplo de 9, ou seja, $a + b = 0$, $9$ ou $18$.
- Se $b = 0$: $a = 0$ ou $a = 9$ → 5040 e 5940.
- Se $b = 5$: $a = 4$ → 5445.

**5.** Por 24, **não necessariamente**: 12 é divisível por 4 e por 6, mas não por 24. Por 12, **sim**: os múltiplos comuns de 4 e 6 são os múltiplos de 12 (que é o [[MMC e MDC|MMC]] de 4 e 6).
**6.** **12.** Com 6 divisores, a fatoração tem a forma $p^5$ (o menor é $2^5 = 32$) ou $p^2 \cdot q$ (o menor é $2^2 \cdot 3 = 12$). Os divisores de 12 são $1, 2, 3, 4, 6, 12$. ✔️

## 🔴 Difícil
**1.** **24 zeros.**
Cada zero no final vem de um fator $10 = 2 \cdot 5$. Há muito mais fatores 2 do que 5, então basta contar os fatores 5:
- múltiplos de 5 até 100: $100 \div 5 = 20$ (cada um dá pelo menos um 5);
- múltiplos de 25 até 100: $100 \div 25 = 4$ (cada um dá um 5 **extra**, pois $25 = 5^2$).

Total: $20 + 4 = 24$.
💡 *Ideia-chave: transformar "contar zeros" em "contar fatores primos".*

**2.** $abab = 1000a + 100b + 10a + b = 1010a + 101b = 101 \cdot (10a + b)$. É sempre $101$ vezes um número, então é divisível por 101. (Exemplo: $3737 = 101 \cdot 37$.)

**3.** Entre dois consecutivos, um é par, então o produto é divisível por 2. Entre três consecutivos, um é múltiplo de 3, então o produto é divisível por 3. Sendo divisível por 2 e por 3, que são primos, é divisível por $2 \cdot 3 = 6$.

**4.** **33.**
- Divisíveis por 2: 50. Divisíveis por 3: 33.
- Os divisíveis **por 2 e por 3** (ou seja, por 6) foram contados duas vezes: são 16.
- Divisíveis por 2 **ou** por 3: $50 + 33 - 16 = 67$.
- Nem por 2 nem por 3: $100 - 67 = 33$.

💡 *Ideia-chave: o princípio da inclusão-exclusão (somar e descontar o que foi contado em dobro), que volta em [[Probabilidade Básica]].*

## 💻 Extra em C#
**1.**
```csharp
bool EhPrimo(int n)
{
    if (n < 2) return false;
    for (int i = 2; i * i <= n; i++)  // i * i <= n é o mesmo que i <= √n
        if (n % i == 0) return false;
    return true;
}
```
**2.** Há **25 primos** até 100.
```csharp
var ehComposto = new bool[101];
var primos = new List<int>();
for (int i = 2; i <= 100; i++)
{
    if (ehComposto[i]) continue;
    primos.Add(i);
    for (int j = i * i; j <= 100; j += i) // risca os múltiplos de i
        ehComposto[j] = true;
}
Console.WriteLine(primos.Count); // 25
```
