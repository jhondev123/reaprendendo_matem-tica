---
tipo: gabarito
tema: Aritmética
conceito: "[[Sistema de Numeração Decimal]]"
tags:
  - aritmetica
  - gabarito
---
# Sistema de Numeração Decimal: Gabarito

**Voltar aos exercícios:** [[Sistema de Numeração Decimal - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** 7.000 (o 7 está na unidade de milhar).
**2.** Três milhões, quarenta mil, quinhentos e seis.
**3.** 12.300.008
**4.** $8 \cdot 1000 + 0 \cdot 100 + 9 \cdot 10 + 3 \cdot 1$
**5.** 345 dezenas (porque $3450 = 345 \cdot 10$).
**6.** 9.876
**7.** 10.000
**8.** 1.000 vezes ($6000 \div 6 = 1000$).

## 🟡 Médio
**1.** Maior: **7.310** (algarismos em ordem decrescente). Menor: **1.037** (o 0 não pode ficar na frente, então começa pelo 1 e o 0 vem logo depois). Diferença: $7310 - 1037 = 6273$.
**2.** $400 + 120 + 15 = 535$. As dezenas e unidades "a mais" se reagrupam.
**3.** São **900** números (de 100 a 999). Metade é par: **450**.
**4.** $25 = 16 + 8 + 1 \Rightarrow 11001_2$. Por divisões: 25→12 (resto 1), 12→6 (0), 6→3 (0), 3→1 (1), 1→0 (1). Lendo os restos de baixo para cima: 11001.
**5.** $32 + 0 + 8 + 4 + 0 + 1 = 45$
**6.** De 1 a 9: $9 \cdot 1 = 9$. De 10 a 99: $90 \cdot 2 = 180$. O 100: 3. Total: $9 + 180 + 3 = 192$.

## 🔴 Difícil
**1.** **140.**
- De 1 a 99: o 1 aparece nas unidades em 1, 11, 21, …, 91 (**10 vezes**) e nas dezenas em 10 a 19 (**10 vezes**). São 20.
- De 100 a 199: o 1 está na casa das centenas em todos os **100** números. Nas dezenas e unidades, repete-se o padrão de 00 a 99: mais **20**.
- Total: $20 + 100 + 20 = 140$.

**2.** **12, 24, 36 e 48.**
Com dezena $a$ e unidade $b$, o número vale $10a + b$. A condição é $10a + b = 4(a + b) = 4a + 4b$, que simplifica para $6a = 3b$, ou seja, $b = 2a$. Como $b \leq 9$, temos $a \in \{1, 2, 3, 4\}$. Conferindo: $12 = 4 \cdot 3$, $24 = 4 \cdot 6$, $36 = 4 \cdot 9$, $48 = 4 \cdot 12$. ✔️

**3.** **359.**
O número é $100a + 10b + c$ e o trocado é $100c + 10b + a$. A diferença é $99c - 99a = 99(c - a) = 594$, então $c - a = 6$. Como $b = 5$ e $a + b + c = 17$, temos $a + c = 12$. Resolvendo: $c = 9$ e $a = 3$. Conferindo: $953 - 359 = 594$. ✔️
💡 *Ideia-chave: escrever o número na forma posicional transforma o enunciado em contas simples.*

**4.** **7.**
- Os números de 1 a 9 usam 9 algarismos (posições 1 a 9).
- Os de 10 a 99 usam $90 \cdot 2 = 180$ algarismos (posições 10 a 189).
- Faltam $2026 - 189 = 1837$ algarismos, já entre os números de 3 algarismos. Como $1837 = 3 \cdot 612 + 1$, os números de 100 a 711 (que são 612) ocupam 1836 posições, e o algarismo seguinte é o **primeiro** algarismo do próximo número, **712**: o **7**.

## 💻 Extra em C#
**1.**
```csharp
int SomaDosAlgarismos(int n)
{
    int soma = 0;
    while (n > 0)
    {
        soma += n % 10; // último algarismo
        n /= 10;        // remove o último algarismo
    }
    return soma;
}
```
**2.**
```csharp
string ParaBinario(int n)
{
    if (n == 0) return "0";
    var resultado = "";
    while (n > 0)
    {
        resultado = (n % 2) + resultado; // o resto entra à esquerda
        n /= 2;
    }
    return resultado;
}
```
Colocar o resto **à esquerda** a cada passo equivale a "ler os restos de baixo para cima".
