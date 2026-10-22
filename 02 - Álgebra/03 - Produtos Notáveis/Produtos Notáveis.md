---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Quadrado da soma
  - Quadrado da diferença
  - Diferença de quadrados
  - Produto da soma pela diferença
tags:
  - algebra
---
# Produtos Notáveis

> [!abstract] Em uma frase
> Algumas multiplicações aparecem tanto que vale a pena **decorar o resultado**: $(a + b)^2 = a^2 + 2ab + b^2$, $\;(a - b)^2 = a^2 - 2ab + b^2$ e $(a + b)(a - b) = a^2 - b^2$. Elas economizam tempo e, lidas ao contrário, viram [[Fatoração]].

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Monômios e Polinômios]] · **Próximo:** [[Fatoração]]
**Praticar:** [[Produtos Notáveis - Exercícios]] · [[Produtos Notáveis - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Desenvolver os três produtos notáveis principais **de cabeça**.
- Explicar $(a + b)^2$ com um desenho de áreas.
- Usar produtos notáveis em contas numéricas ($51^2$, $99 \cdot 101$).
- Desenvolver o cubo da soma e da diferença.

---

## 1. Por que decorar?

Você **sabe** calcular $(x + 3)^2$: é $(x + 3)(x + 3)$, com o chuveirinho de [[Monômios e Polinômios]]:
$$(x + 3)(x + 3) = x^2 + 3x + 3x + 9 = x^2 + 6x + 9$$

Mas isso aparece **o tempo todo** (em equações, em geometria, no cálculo, em ML). Conhecendo o padrão, você escreve a resposta direto e, mais importante, **reconhece o padrão ao contrário** quando ele aparece numa conta.

## 2. Quadrado da soma

$$(a + b)^2 = a^2 + 2ab + b^2$$

> "O quadrado do primeiro, **mais duas vezes o primeiro pelo segundo**, mais o quadrado do segundo."

> [!example] A prova com um desenho
> Um quadrado de lado $a + b$ pode ser cortado em 4 pedaços:
> ```
>       a         b
>   ┌─────────┬─────┐
> a │   a²    │ ab  │
>   │         │     │
>   ├─────────┼─────┤
> b │   ab    │ b²  │
>   └─────────┴─────┘
> ```
> Área total $= a^2 + ab + ab + b^2 = a^2 + 2ab + b^2$. Os **dois retângulos** $ab$ são o termo que todo mundo esquece!

> [!danger] O "sonho do calouro"
> $$(a + b)^2 \neq a^2 + b^2$$
> Teste com números: $(3 + 4)^2 = 49$, mas $3^2 + 4^2 = 25$. Faltam os $2 \cdot 3 \cdot 4 = 24$. É o mesmo erro de $\sqrt{a + b} \neq \sqrt{a} + \sqrt{b}$ ([[Radiciação]]).

## 3. Quadrado da diferença

$$(a - b)^2 = a^2 - 2ab + b^2$$

Só muda o sinal do termo do meio. (É o quadrado da soma com $-b$ no lugar de $b$, e $(-b)^2 = b^2$.)

$$(x - 5)^2 = x^2 - 10x + 25 \qquad (3a - 2b)^2 = 9a^2 - 12ab + 4b^2$$

> [!warning] Cuidado com o coeficiente
> $(2x + 1)^2$: o "primeiro" é $2x$ **inteiro**. Então $(2x)^2 + 2 \cdot 2x \cdot 1 + 1^2 = 4x^2 + 4x + 1$. Não esqueça de elevar o 2 também.

## 4. Produto da soma pela diferença

$$(a + b)(a - b) = a^2 - b^2$$

> "O quadrado do primeiro **menos** o quadrado do segundo."

Os termos do meio se cancelam: $(a + b)(a - b) = a^2 - ab + ab - b^2$. Esse produto se chama **diferença de quadrados**.

$$(x + 4)(x - 4) = x^2 - 16 \qquad (\sqrt{3} + \sqrt{2})(\sqrt{3} - \sqrt{2}) = 3 - 2 = 1$$

O segundo exemplo é o **conjugado**, usado para racionalizar denominadores (em [[Expoentes e Radicais com Variáveis]]).

## 5. Cubos (menos frequentes, mas úteis)

$$(a + b)^3 = a^3 + 3a^2b + 3ab^2 + b^3 \qquad (a - b)^3 = a^3 - 3a^2b + 3ab^2 - b^3$$

Os coeficientes 1, 3, 3, 1 vêm do **triângulo de Pascal**, que aparece em [[Binômio de Newton]].

## 6. Contas de cabeça

| Conta | Truque | Resultado |
|---|---|---|
| $51^2$ | $(50 + 1)^2 = 2500 + 100 + 1$ | $2601$ |
| $49^2$ | $(50 - 1)^2 = 2500 - 100 + 1$ | $2401$ |
| $99 \cdot 101$ | $(100 - 1)(100 + 1) = 10000 - 1$ | $9999$ |
| $2026^2 - 2025^2$ | $(2026 - 2025)(2026 + 2025)$ | $4051$ |

> [!question]- Tente agora (clique para ver as respostas)
> (a) $(x - 7)^2$ (b) $(5 + 2y)(5 - 2y)$ (c) $102^2$
> **Respostas:** (a) $x^2 - 14x + 49$ (b) $25 - 4y^2$ (c) $(100 + 2)^2 = 10404$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: com frações
> $$\left(\frac{x}{2} + \frac{1}{3}\right)^2 = \frac{x^2}{4} + 2 \cdot \frac{x}{2} \cdot \frac{1}{3} + \frac{1}{9} = \frac{x^2}{4} + \frac{x}{3} + \frac{1}{9}$$

> [!example] Exemplo 2: com raiz
> $(\sqrt{5} + 1)^2 = 5 + 2\sqrt{5} + 1 = 6 + 2\sqrt{5}$

> [!example] Exemplo 3: simplificar
> $(x + 1)^2 - (x - 1)^2 = (x^2 + 2x + 1) - (x^2 - 2x + 1) = 4x$

> [!example] Exemplo 4: usando sem saber $a$ e $b$
> Se $a + b = 7$ e $ab = 10$, quanto vale $a^2 + b^2$?
> $(a + b)^2 = a^2 + b^2 + 2ab \Rightarrow 49 = a^2 + b^2 + 20 \Rightarrow a^2 + b^2 = 29$

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $(x + 3)^2 = x^2 + 9$ | $x^2 + 6x + 9$ | faltou o $2ab$ |
| $(x - 3)^2 = x^2 - 9$ | $x^2 - 6x + 9$ | isso é $(x + 3)(x - 3)$ |
| $(2x + 1)^2 = 2x^2 + 4x + 1$ | $4x^2 + 4x + 1$ | $(2x)^2 = 4x^2$ |
| $(x - 3)^2 = x^2 - 6x - 9$ | $\dots + 9$ | $(-3)^2 = +9$ |
| $-(x - 1)^2 = -x^2 - 2x + 1$ | $-x^2 + 2x - 1$ | desenvolva primeiro e só depois troque **todos** os sinais |

---

## 💻 Conexão com programação e ML

- **Em ML, o quadrado da diferença está em todo lugar.** O erro quadrático é $(y - \hat{y})^2 = y^2 - 2y\hat{y} + \hat{y}^2$.
- **Distâncias rápidas:** a distância ao quadrado entre dois vetores é $\lVert a - b \rVert^2 = \lVert a \rVert^2 - 2\,a \cdot b + \lVert b \rVert^2$, o quadrado da diferença para vetores. Bibliotecas de k-NN usam exatamente essa expansão para calcular milhões de distâncias com uma única multiplicação de matrizes ([[Produto Escalar e Normas]]).
- **Variância:** a fórmula "média dos quadrados menos o quadrado da média" ($\overline{x^2} - \bar{x}^2$) sai do quadrado da diferença ([[Medidas de Dispersão]]).

---

## 🔗 Conexões
- **Usa:** [[Monômios e Polinômios]] (é só multiplicação de polinômios), [[Potenciação]].
- **É usado em:**
  - [[Fatoração]]: lendo as fórmulas ao contrário.
  - [[Expoentes e Radicais com Variáveis]]: racionalização com conjugado.
  - [[Equações do 2º Grau]]: completar o quadrado e chegar à fórmula de Bhaskara.
- **Mais adiante:** [[Binômio de Newton]] (a generalização de $(a + b)^n$), [[Distância entre Pontos]] e [[Equação da Circunferência]] (aparecem $(x - a)^2$), [[Produto Escalar e Normas]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Escreva as três fórmulas principais em palavras.
2. Desenhe o quadrado que prova $(a + b)^2 = a^2 + 2ab + b^2$.
3. Por que $(a + b)^2 \neq a^2 + b^2$? Dê um exemplo numérico.
4. Desenvolva $(3x - 1)^2$ e $(x^2 + 2)(x^2 - 2)$.
5. Calcule $31^2$ e $48 \cdot 52$ de cabeça.
6. Se $x - y = 3$ e $xy = 4$, quanto vale $x^2 + y^2$?
