---
tipo: gabarito
tema: Aritmética
conceito: "[[Porcentagem]]"
tags:
  - aritmetica
  - gabarito
---
# Porcentagem: Gabarito

**Voltar aos exercícios:** [[Porcentagem - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** (a) $\frac{35}{100} = \frac{7}{20} = 0{,}35$ (b) 8% (c) $3 \div 8 = 0{,}375 = 37{,}5\%$
**2.** $0{,}15 \cdot 200 = 30$
**3.** 36; 18; 3,6
**4.** $\frac{18}{72} = \frac{1}{4} = 25\%$
**5.** $80 \cdot 0{,}75 = $ R\$ 60
**6.** $2500 \cdot 1{,}08 = $ R\$ 2.700
**7.** (a) 1,12 (b) 0,65 (c) 2,5
**8.** $1{,}2 \cdot 50 = 60$

## 🟡 Médio
**1.** $1{,}1 \cdot 0{,}9 = 0{,}99$: queda de **1%**.
**2.** $\frac{1200}{0{,}8} = $ **R\$ 1.500**
**3.** $\frac{34 - 40}{40} = -0{,}15$: queda de **15%**.
**4.** **8 p.p.** e **10%** ($\frac{8}{80} = 0{,}1$).
**5.** $0{,}125 \cdot 0{,}75 \cdot 0{,}8 = 0{,}075 = \frac{3}{40}$. (Com frações: $\frac{1}{8} \cdot \frac{3}{4} \cdot \frac{4}{5} = \frac{3}{40}$.)
**6.** $J = 2000 \cdot 0{,}015 \cdot 8 = 240$, então $M = $ **R\$ 2.240**.
**7.** $1000 \cdot 1{,}1^3 = 1000 \cdot 1{,}331 = $ **R\$ 1.331**
**8.** $0{,}1 \cdot 0{,}9^3 = 0{,}1 \cdot 0{,}729 = 0{,}0729$. A taxa ficou em 72,9% do valor inicial, uma redução de **27,1%**.

## 🔴 Difícil
**1.** **20%.**
O fator de volta deve desfazer o 1,25: $\frac{1}{1{,}25} = 0{,}8$, ou seja, uma queda de 20%. (Por exemplo: 100 → 125 → 100, e 25 é 20% de 125.)

**2.** **16 litros.**
Há $0{,}3 \cdot 40 = 12$ L de álcool e 28 L de água. A **água não muda**. Para ela ser 50% da mistura, o total tem que ser $2 \cdot 28 = 56$ L. Então é preciso acrescentar $56 - 40 = 16$ L de álcool. (Conferindo: $\frac{12 + 16}{56} = \frac{28}{56} = 50\%$. ✔️)
💡 *Ideia-chave: procure a parte que **não muda**.*

**3.** **5 kg.**
A parte que **não é água** tem $1\% \cdot 10 = 0{,}1$ kg e não evapora. Depois de secar, ela passa a ser $2\%$ da melancia: $0{,}02 \cdot M = 0{,}1 \Rightarrow M = 5$ kg. A melancia perdeu **metade** da massa para que a porcentagem de água caísse só um ponto percentual!
💡 *Mesma ideia-chave do problema anterior.*

**4.** **1.000 alunos.**
$1{,}2 \cdot 0{,}8 = 0{,}96$, então $0{,}96 \cdot x = 960$ e $x = 1000$.

## 💻 Extra em C#
**1.**
```csharp
double FatorAcumulado(params double[] variacoes)
{
    double fator = 1;
    foreach (var v in variacoes) fator *= 1 + v;
    return fator;
}
```
(Com `double`, o resultado pode aparecer como `0.9900000000000001`. Lembra de [[Números Decimais]]?)
**2.**
```csharp
double m = 1000;
for (int i = 0; i < 12; i++) m *= 1.01;
double m2 = 1000 * Math.Pow(1.01, 12);
// os dois dão aproximadamente 1126,83
```
