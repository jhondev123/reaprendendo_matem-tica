---
tipo: exercicios
tema: Aritmética
conceito: "[[Radiciação]]"
tags:
  - aritmetica
  - exercicios
---
# Radiciação: Exercícios

**Teoria:** [[Radiciação]] · **Gabarito:** [[Radiciação - Gabarito]]

> [!info] Como fazer
> Resolva no caderno. Dê as respostas na forma **exata e simplificada** (por exemplo, $6\sqrt{2}$, e não 8,49), a não ser que o exercício peça um valor aproximado. Corrija ao fim de cada bloco e marque o checkbox das que acertou. Errou? Registre no [[Caderno de Erros]] e refaça amanhã.

## 🟢 Fácil
- [ ] **1.** Calcule: $\sqrt{81}$, $\;\sqrt[3]{27}$, $\;\sqrt[3]{-64}$, $\;\sqrt[4]{16}$, $\;\sqrt{0}$
- [ ] **2.** Calcule: $\sqrt{\frac{4}{9}}$, $\;\sqrt{0{,}49}$, $\;\sqrt{1{,}44}$
- [ ] **3.** Entre quais inteiros consecutivos estão $\sqrt{50}$ e $\sqrt{120}$?
- [ ] **4.** Simplifique: $\sqrt{12}$, $\;\sqrt{50}$, $\;\sqrt{72}$
- [ ] **5.** $3\sqrt{2} + 5\sqrt{2} - \sqrt{2}$
- [ ] **6.** Calcule: (a) $\sqrt{3} \cdot \sqrt{12}$ (b) $\sqrt{50} \div \sqrt{2}$
- [ ] **7.** (a) Escreva $\sqrt{5}$ e $\sqrt[3]{7^2}$ como potências. (b) Calcule $8^{1/3}$ e $16^{3/4}$.
- [ ] **8.** $\sqrt{-16}$ existe nos reais? E $\sqrt[3]{-8}$? Justifique.

## 🟡 Médio
- [ ] **1.** $\sqrt{8} + \sqrt{18} - \sqrt{32}$
- [ ] **2.** Racionalize: (a) $\frac{1}{\sqrt{2}}$ (b) $\frac{6}{\sqrt{3}}$ (c) $\frac{10}{3\sqrt{5}}$
- [ ] **3.** 🔀 $\sqrt{0{,}25} + \sqrt[3]{-0{,}125} - \left(\frac{1}{2}\right)^{-1}$
- [ ] **4.** 🔀 $\sqrt{0{,}\overline{4}} + \sqrt[3]{\frac{8}{27}}$
- [ ] **5.** 🔀 $\left(\sqrt{2} + \sqrt{8}\right)^2$
- [ ] **6.** 🔀 $27^{2/3} - 16^{-1/2} + 0{,}01^{1/2}$ (dê a resposta como fração irredutível)
- [ ] **7.** Um quadrado tem área de 72 cm². Qual é a medida exata do lado? E a aproximada, com duas casas decimais (use $\sqrt{2} \approx 1{,}414$)?
- [ ] **8.** 🔀 $\left[\sqrt{3^2 + 4^2} - \sqrt{9} - \sqrt{16}\right] \cdot \sqrt{\frac{1}{4}}$

## 🔴 Difícil (estilo OBMEP)
- [ ] **1.** Simplifique $\sqrt{7 + 4\sqrt{3}}$. (Dica: procure um número da forma $a + \sqrt{3}$ cujo quadrado seja $7 + 4\sqrt{3}$.)
- [ ] **2.** Qual é maior: $\sqrt{5} + \sqrt{7}$ ou $\sqrt{3} + \sqrt{9}$? Justifique **sem calculadora**.
- [ ] **3.** Quantos números inteiros existem entre $\sqrt{20}$ e $\sqrt{200}$?
- [ ] **4.** Calcule $\dfrac{1}{\sqrt{1} + \sqrt{2}} + \dfrac{1}{\sqrt{2} + \sqrt{3}} + \dots + \dfrac{1}{\sqrt{99} + \sqrt{100}}$. (Dica: $(\sqrt{b} + \sqrt{a})(\sqrt{b} - \sqrt{a}) = b - a$.)

## 💻 Extra em C# (opcional)
- [ ] **1.** Implemente `double RaizBabilonica(double a)` com o método babilônico: comece com `x = a` e repita `x = (x + a / x) / 2` até a diferença entre duas iterações ser menor que `1e-12`. Quantas iterações são necessárias para $a = 2$?
- [ ] **2.** Rode e explique: `Math.Sqrt(-1)`, `Math.Pow(-8, 1.0 / 3)` e `Math.Cbrt(-8)`.

## 🏅 Teste-se com provas reais
OBMEP **Nível 2 e 3**: comparação de radicais e simplificação de raízes "aninhadas". Links em [[Provas e Olimpíadas]].
