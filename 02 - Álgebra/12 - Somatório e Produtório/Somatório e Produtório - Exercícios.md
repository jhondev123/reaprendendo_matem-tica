---
tipo: exercicios
tema: Álgebra
conceito: "[[Somatório e Produtório]]"
tags:
  - algebra
  - exercicios
---
# Somatório e Produtório: Exercícios

**Teoria:** [[Somatório e Produtório]] · **Gabarito:** [[Somatório e Produtório - Gabarito]]

> [!info] Como fazer
> Na dúvida, **abra o somatório** (escreva os termos um por um). Corrija ao fim de cada bloco e marque o checkbox das que acertou. Errou? Registre no [[Caderno de Erros]] e refaça amanhã.

## 🟢 Fácil
- [ ] **1.** $\displaystyle\sum_{i=1}^{5} i$
- [ ] **2.** $\displaystyle\sum_{k=1}^{4} k^2$
- [ ] **3.** $\displaystyle\sum_{i=1}^{3} (2i + 1)$
- [ ] **4.** $\displaystyle\sum_{i=1}^{10} 7$
- [ ] **5.** Escreva com $\Sigma$: $2 + 4 + 6 + \dots + 20$
- [ ] **6.** Escreva com $\Sigma$: $1 + \frac{1}{2} + \frac{1}{3} + \dots + \frac{1}{100}$
- [ ] **7.** Calcule $\displaystyle\prod_{i=1}^{4} i$ e $\displaystyle\prod_{i=1}^{3} 2$.
- [ ] **8.** Quantos termos tem $\displaystyle\sum_{i=3}^{12} x_i$?

## 🟡 Médio
- [ ] **1.** Para $x = (2, 5, 3, 8, 7)$, calcule: $\sum x_i$, a média $\bar{x}$, $\sum x_i^2$ e $\left(\sum x_i\right)^2$.
- [ ] **2.** Se $\sum_{i=1}^{20} a_i = 50$ e $\sum_{i=1}^{20} b_i = 30$, calcule $\sum_{i=1}^{20} (3a_i - 2b_i + 1)$.
- [ ] **3.** Calcule $\sum_{i=1}^{100} i$ e $\sum_{i=1}^{50} (2i - 1)$.
- [ ] **4.** Valores reais $y = (3, 5, 2)$ e previsões $\hat{y} = (2, 5, 4)$. Calcule o MSE $= \frac{1}{n}\sum (y_i - \hat{y}_i)^2$.
- [ ] **5.** Para $\mathbf{w} = (0{,}5;\ -1;\ 2)$ e $\mathbf{x} = (4;\ 3;\ 1{,}5)$, calcule o produto escalar $\sum w_j x_j$ e a saída do neurônio $z = \sum w_j x_j + b$ com $b = -0{,}5$.
- [ ] **6.** 🔀 $\displaystyle\sum_{k=1}^{4} \left(\frac{1}{2}\right)^k$
- [ ] **7.** 🔀 $\displaystyle\sum_{i=1}^{4} (-1)^i \cdot i$
- [ ] **8.** 🔀 $\displaystyle\sum_{k=1}^{99} \frac{1}{k(k+1)}$

## 🔴 Difícil (estilo OBMEP)
- [ ] **1.** Calcule $\sum_{i=1}^{n} (2i - 1)$ em função de $n$ e explique o resultado com um desenho de quadrados.
- [ ] **2.** Prove que, para quaisquer valores $x_1, \dots, x_n$ com média $\bar{x}$, vale $\sum_{i=1}^{n} (x_i - \bar{x}) = 0$. (Os desvios em relação à média sempre somam zero.)
- [ ] **3.** Calcule $\displaystyle\sum_{i=1}^{10} \sum_{j=1}^{10} i \cdot j$.
- [ ] **4.** Calcule $\displaystyle\prod_{k=2}^{100} \left(1 - \frac{1}{k^2}\right)$.

## 💻 Extra em C# (opcional)
- [ ] **1.** Escreva `double Mse(double[] y, double[] yHat)` e `double ProdutoEscalar(double[] w, double[] x)`, com laços e depois com LINQ.
- [ ] **2.** Multiplique 1.000 probabilidades iguais a 0,01 com `double`. O que acontece? Agora some os logaritmos (`Math.Log`) e compare.

## 🏅 Teste-se com provas reais
OBMEP **Nível 2 e 3**: somas de sequências, somas telescópicas e produtos que se cancelam. Links em [[Provas e Olimpíadas]].
