---
tipo: gabarito
tema: Aritmética
conceito: "[[Frações e Equivalência]]"
tags:
  - aritmetica
  - gabarito
---
# Frações e Equivalência: Gabarito

**Voltar aos exercícios:** [[Frações e Equivalência - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** Comeu $\frac{3}{8}$; sobraram $\frac{5}{8}$.
**2.** Por exemplo, $\frac{4}{10}, \frac{6}{15}, \frac{20}{50}$.
**3.** (a) $\frac{3}{4}$ (mdc 12)  (b) $\frac{3}{4}$ (mdc 15)  (c) $\frac{3}{7}$ (mdc 14)
**4.** $17 = 5 \cdot 3 + 2 \Rightarrow 3\frac{2}{5}$. E $2\frac{3}{4} = \frac{2 \cdot 4 + 3}{4} = \frac{11}{4}$.
**5.** (a) $<$  (b) $>$  (c) $=$
**6.** $60 \div 4 \cdot 3 = 45$
**7.** $\frac{12}{4} = 3$ e $\frac{20}{5} = 4$.
**8.** $\frac{7}{4} = 1{,}75$ fica entre **1 e 2**; $-\frac{5}{3} \approx -1{,}67$ fica entre **−2 e −1**.

## 🟡 Médio
**1.** O MMC de 3, 5, 8 e 12 é 120: $\frac{80}{120}, \frac{72}{120}, \frac{75}{120}, \frac{70}{120}$. Ordem: $\frac{7}{12} < \frac{3}{5} < \frac{5}{8} < \frac{2}{3}$.
**2.** (a) $56 = 8 \cdot 7 \Rightarrow x = 21$  (b) $15 = 5 \cdot 3 \Rightarrow x = 7 \cdot 3 = 21$
**3.** $\text{mdc}(168, 240) = 24$, então $\frac{168}{240} = \frac{7}{10}$.
**4.** $\frac{25}{60} = \frac{5}{12}$ de hora; $\frac{8}{24} = \frac{1}{3}$ do dia.
**5.** Reescreva com um denominador maior: $\frac{1}{3} = \frac{4}{12}$ e $\frac{1}{2} = \frac{6}{12}$, então $\frac{5}{12}$ está entre elas. Com denominador 24: $\frac{8}{24}$ e $\frac{12}{24}$, e servem $\frac{9}{24}, \frac{10}{24}, \frac{11}{24}$. Há **infinitas** respostas, por exemplo $\frac{5}{12}$ e $\frac{2}{5}$.
**6.** (a) Cortando $2^2$ e $3^2$: $\frac{2 \cdot 5}{3} = \frac{10}{3}$  (b) $\frac{18}{-24} = -\frac{3}{4}$
**7.** (a) $\frac{12 - 8}{9 - 1} = \frac{4}{8} = \frac{1}{2}$  (b) $\frac{-8}{-12} = \frac{2}{3}$  (c) $\frac{9 - 3}{12} = \frac{6}{12} = \frac{1}{2}$

## 🔴 Difícil
**1.** **4 frações.** O numerador vai de 1 a 11 e não pode ter fator comum com $12 = 2^2 \cdot 3$, ou seja, não pode ser par nem múltiplo de 3. Sobram 1, 5, 7 e 11: $\frac{1}{12}, \frac{5}{12}, \frac{7}{12}, \frac{11}{12}$.

**2.** $\frac{5}{7}$.
Queremos $\frac{x}{7} > \frac{5}{8}$. Pela multiplicação cruzada, $8x > 35$, então $x > 4{,}375$. O menor inteiro possível é $x = 5$. Conferindo: $\frac{4}{7} \approx 0{,}571 < 0{,}625 < \frac{5}{7} \approx 0{,}714$. ✔️

**3.** **7.**
Testando: $\frac{3+1}{5+1} = \frac{4}{6}$, $\frac{5}{7}$, $\frac{6}{8}$, $\frac{7}{9}$, $\frac{8}{10}$, $\frac{9}{11}$, $\frac{10}{12} = \frac{5}{6}$ ✔️.
(Com álgebra, que você vai ver em [[Equações do 1º Grau]]: $\frac{3+n}{5+n} = \frac{5}{6} \Rightarrow 18 + 6n = 25 + 5n \Rightarrow n = 7$.)

**4.** **4 frações.**
Como $b = 30 - a$, um fator comum de $a$ e $b$ também divide $a + b = 30$. Então $\frac{a}{b}$ é irredutível exatamente quando $a$ não tem fator comum com $30 = 2 \cdot 3 \cdot 5$. Para a fração ser menor que 1, precisamos de $a < b$, ou seja, $a < 15$. Entre 1 e 14, os que não são divisíveis por 2, 3 ou 5 são **1, 7, 11 e 13**: $\frac{1}{29}, \frac{7}{23}, \frac{11}{19}, \frac{13}{17}$.
💡 *Ideia-chave: $\text{mdc}(a, b) = \text{mdc}(a, a + b)$.*

## 💻 Extra em C#
```csharp
record struct Fracao(long Num, long Den)
{
    public Fracao Simplificar()
    {
        long d = Mdc(Math.Abs(Num), Math.Abs(Den));
        long sinal = Den < 0 ? -1 : 1; // sinal sempre no numerador
        return new Fracao(sinal * Num / d, sinal * Den / d);
    }

    static long Mdc(long a, long b) => b == 0 ? a : Mdc(b, a % b);
}

int Comparar(Fracao a, Fracao b)
{
    // supõe denominadores positivos (garantido por Simplificar)
    long esquerda = a.Num * b.Den;
    long direita = b.Num * a.Den;
    return esquerda.CompareTo(direita);
}
```
