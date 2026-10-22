---
tipo: gabarito
tema: Álgebra
conceito: "[[Somatório e Produtório]]"
tags:
  - algebra
  - gabarito
---
# Somatório e Produtório: Gabarito

**Voltar aos exercícios:** [[Somatório e Produtório - Exercícios]]

> [!warning] Só abra depois de tentar
> Conferir a resposta antes de tentar de verdade elimina justamente o esforço que faz você aprender.

## 🟢 Fácil
**1.** $15$
**2.** $1 + 4 + 9 + 16 = 30$
**3.** $3 + 5 + 7 = 15$
**4.** $70$
**5.** $\sum_{i=1}^{10} 2i$
**6.** $\sum_{k=1}^{100} \frac{1}{k}$
**7.** $24$ e $8$
**8.** $12 - 3 + 1 = 10$ termos

## 🟡 Médio
**1.** $\sum x_i = 25$; $\;\bar{x} = 5$; $\;\sum x_i^2 = 4 + 25 + 9 + 64 + 49 = 151$; $\;\left(\sum x_i\right)^2 = 625$. (Bem diferentes!)
**2.** $150 - 60 + 20 = 110$
**3.** $\frac{100 \cdot 101}{2} = 5050$. E $2 \sum_{i=1}^{50} i - \sum_{i=1}^{50} 1 = 2 \cdot 1275 - 50 = 2500$ (que é $50^2$).
**4.** Erros: $1, 0, -2$. Quadrados: $1, 0, 4$. MSE $= \frac{5}{3} \approx 1{,}67$.
**5.** $0{,}5 \cdot 4 + (-1) \cdot 3 + 2 \cdot 1{,}5 = 2 - 3 + 3 = 2$; $\;z = 2 - 0{,}5 = 1{,}5$
**6.** $\frac{8 + 4 + 2 + 1}{16} = \frac{15}{16}$
**7.** $-1 + 2 - 3 + 4 = 2$
**8.** Telescópica: $1 - \frac{1}{100} = \frac{99}{100}$

## 🔴 Difícil
**1.** $n^2$.
$\sum (2i - 1) = 2\sum i - \sum 1 = 2 \cdot \frac{n(n + 1)}{2} - n = n^2 + n - n = n^2$.
**Desenho:** comece com 1 quadradinho. Para formar um quadrado $2 \times 2$, acrescente um "L" de 3; para $3 \times 3$, um "L" de 5; e assim por diante. Cada "L" é o próximo ímpar, e somando os $n$ primeiros ímpares você monta um quadrado $n \times n$.

**2.**
$$\sum_{i=1}^{n} (x_i - \bar{x}) = \sum_{i=1}^{n} x_i - \sum_{i=1}^{n} \bar{x} = n\bar{x} - n\bar{x} = 0$$
Usamos que $\sum x_i = n\bar{x}$ (da definição de média) e que $\bar{x}$ é **constante** em relação a $i$. (Por isso a variância usa os desvios **ao quadrado**: sem o quadrado, a soma sempre daria zero. Veja [[Medidas de Dispersão]].)

**3.** **3025.**
Como $i$ não depende de $j$: $\sum_i \sum_j i \cdot j = \sum_i \left(i \sum_j j\right) = \left(\sum_i i\right)\left(\sum_j j\right) = 55 \cdot 55 = 3025$.
(Aqui o produto das somas **vale**, porque cada termo é um produto de uma parte só com $i$ e outra só com $j$.)

**4.** $\frac{101}{200}$.
$1 - \frac{1}{k^2} = \frac{k^2 - 1}{k^2} = \frac{(k - 1)(k + 1)}{k \cdot k}$. Separando em dois produtórios telescópicos:
- $\prod_{k=2}^{100} \frac{k - 1}{k} = \frac{1}{2} \cdot \frac{2}{3} \cdots \frac{99}{100} = \frac{1}{100}$
- $\prod_{k=2}^{100} \frac{k + 1}{k} = \frac{3}{2} \cdot \frac{4}{3} \cdots \frac{101}{100} = \frac{101}{2}$

Resultado: $\frac{1}{100} \cdot \frac{101}{2} = \frac{101}{200}$.

## 💻 Extra em C#
**1.**
```csharp
double Mse(double[] y, double[] yHat)
    => y.Zip(yHat, (a, b) => (a - b) * (a - b)).Average();

double ProdutoEscalar(double[] w, double[] x)
    => w.Zip(x, (a, b) => a * b).Sum();
```
**2.** O produto $0{,}01^{1000} = 10^{-2000}$ é menor que o menor `double` positivo (cerca de $10^{-308}$), então o resultado vira `0` (*underflow*). A soma dos logaritmos dá $1000 \cdot \ln 0{,}01 \approx -4605{,}17$, um número perfeitamente representável. É por isso que modelos maximizam a **log**-verossimilhança.
