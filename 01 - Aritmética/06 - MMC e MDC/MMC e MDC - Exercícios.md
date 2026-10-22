---
tipo: exercicios
tema: Aritmética
conceito: "[[MMC e MDC]]"
tags:
  - aritmetica
  - exercicios
---
# MMC e MDC: Exercícios

**Teoria:** [[MMC e MDC]] · **Gabarito:** [[MMC e MDC - Gabarito]]

> [!info] Como fazer
> Resolva no caderno, mostrando as contas. Nos problemas, **escreva primeiro se é MMC ou MDC e por quê**. Corrija ao fim de cada bloco e marque o checkbox das que acertou. Errou? Registre no [[Caderno de Erros]] e refaça amanhã.

## 🟢 Fácil
- [ ] **1.** Calcule $\text{mmc}(4, 6)$ e $\text{mdc}(4, 6)$ listando múltiplos e divisores.
- [ ] **2.** Calcule $\text{mmc}(12, 18)$ e $\text{mdc}(12, 18)$ pela fatoração.
- [ ] **3.** $\text{mmc}(8, 12, 20)$
- [ ] **4.** $\text{mdc}(36, 60, 84)$
- [ ] **5.** Calcule $\text{mdc}(252, 198)$ pelo algoritmo de Euclides.
- [ ] **6.** 15 e 28 são primos entre si? Quanto vale $\text{mmc}(15, 28)$?
- [ ] **7.** Use o MDC para simplificar $\dfrac{84}{126}$ de uma vez só.
- [ ] **8.** Dois números têm $\text{mmc} = 60$ e $\text{mdc} = 4$. Um deles é 12. Qual é o outro?

## 🟡 Médio
- [ ] **1.** Três luzes piscam a cada 6, 8 e 10 segundos. Elas acabaram de piscar juntas. Em quanto tempo piscarão juntas de novo?
- [ ] **2.** Uma loja tem 48 camisetas brancas e 72 pretas e quer montar o **maior número possível** de kits iguais, sem sobrar nenhuma camiseta. Quantos kits? O que vai em cada um?
- [ ] **3.** Qual é a proporção mais simples de uma tela de $1920 \times 1080$? E de uma de $1280 \times 1024$?
- [ ] **4.** Um terreno retangular de 120 m por 84 m será cercado com estacas igualmente espaçadas, com uma estaca em cada canto e a **maior distância possível** entre elas. Quantas estacas serão usadas?
- [ ] **5.** Qual é o menor número natural que, dividido por 12, por 15 e por 20, deixa sempre **resto 7**?
- [ ] **6.** Numa pista, Ana completa uma volta em 72 s e Bruno, em 96 s. Eles partem juntos da largada. Depois de quanto tempo passam juntos pela largada de novo? Quantas voltas cada um terá dado?

## 🔴 Difícil (estilo OBMEP)
- [ ] **1.** Qual é o menor número natural que deixa resto 1 quando dividido por 2, 3, 4, 5 e 6, e que é divisível por 7?
- [ ] **2.** Dois números naturais somam 84 e o MDC deles é 12. Quais são **todos** os pares possíveis?
- [ ] **3.** Uma engrenagem A, com 24 dentes, gira encaixada numa engrenagem B, com 36 dentes. Marcamos com tinta os dois dentes que estão se tocando. Depois de quantas voltas de A as duas marcas voltam a se tocar? E quantas voltas terá dado B?
- [ ] **4.** Calcule $\text{mdc}(2^{10} - 1,\; 2^{6} - 1)$, ou seja, $\text{mdc}(1023, 63)$, pelo algoritmo de Euclides.

## 💻 Extra em C# (opcional)
- [ ] **1.** Implemente `Mdc(int a, int b)` pelo algoritmo de Euclides (com recursão ou com um laço) e `Mmc(int a, int b)` usando a relação mmc · mdc = a · b.
- [ ] **2.** Escreva `string Proporcao(int largura, int altura)`, que devolve `"16:9"` para `(1920, 1080)`.

## 🏅 Teste-se com provas reais
OBMEP **Nível 1 e 2**: problemas de "encontros" (MMC) e "cortes iguais" (MDC). Links em [[Provas e Olimpíadas]].
