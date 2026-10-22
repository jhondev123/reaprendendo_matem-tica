---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Potências com letras
  - Radicais algébricos
  - Conjugado
  - Racionalização com conjugado
tags:
  - algebra
---
# Expoentes e Radicais com Variáveis

> [!abstract] Em uma frase
> As propriedades de [[Potenciação]] e [[Radiciação]] valem igualzinho com letras. O grande truque é **converter tudo para potência** ($\sqrt{x} = x^{1/2}$, $\frac{1}{x^2} = x^{-2}$): aí basta somar e subtrair expoentes.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Potenciação]], [[Radiciação]], [[Produtos Notáveis]] · **Próximo:** [[Equações do 2º Grau]]
**Praticar:** [[Expoentes e Radicais com Variáveis - Exercícios]] · [[Expoentes e Radicais com Variáveis - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Simplificar expressões com potências de expoente inteiro, negativo e fracionário.
- Converter entre radical e potência.
- Simplificar radicais com variáveis.
- **Racionalizar** usando o **conjugado**.
- Reescrever uma expressão como soma de termos $a \cdot x^n$, que é a forma que o cálculo usa.

---

## 1. As mesmas propriedades, agora com letras

| Propriedade | Exemplo |
|---|---|
| $x^m \cdot x^n = x^{m+n}$ | $x^3 \cdot x^5 = x^8$ |
| $\dfrac{x^m}{x^n} = x^{m-n}$ | $\dfrac{a^7}{a^4} = a^3$ |
| $(x^m)^n = x^{mn}$ | $(y^2)^4 = y^8$ |
| $(xy)^n = x^n y^n$ | $(2x^3y)^2 = 4x^6y^2$ |
| $x^{-n} = \dfrac{1}{x^n}$ | $x^{-3} = \dfrac{1}{x^3}$ |
| $x^{m/n} = \sqrt[n]{x^m}$ | $x^{2/3} = \sqrt[3]{x^2}$ |

> [!example] Passo a passo com expoente negativo
> $$(x^2y^{-1})^{-2} \cdot x^3y$$
> 1. Potência de potência (o $-2$ multiplica cada expoente): $x^{-4}y^{2}$
> 2. Multiplique, somando os expoentes de cada letra: $x^{-4+3}\,y^{2+1} = x^{-1}y^3$
> 3. Escreva sem expoente negativo: $\dfrac{y^3}{x}$

## 2. Radical ↔ potência

| Radical | Potência |
|---|---|
| $\sqrt{x}$ | $x^{1/2}$ |
| $\sqrt[3]{x^2}$ | $x^{2/3}$ |
| $\dfrac{1}{\sqrt{x}}$ | $x^{-1/2}$ |
| $x\sqrt{x}$ | $x^1 \cdot x^{1/2} = x^{3/2}$ |

**Por que converter?** Porque multiplicar radicais de **índices diferentes** fica fácil:
$$\sqrt{x} \cdot \sqrt[3]{x} = x^{1/2} \cdot x^{1/3} = x^{\frac{1}{2} + \frac{1}{3}} = x^{5/6} = \sqrt[6]{x^5}$$

> [!important] $\sqrt{x^2} = \lvert x \rvert$
> Se $x = -3$: $\sqrt{(-3)^2} = \sqrt{9} = 3 = \lvert -3 \rvert$. Nos exercícios, quando aparecer "$x \geq 0$", você pode escrever simplesmente $\sqrt{x^2} = x$.

## 3. Simplificando radicais com variáveis (com $x \geq 0$)

A ideia é a mesma de $\sqrt{72} = 6\sqrt{2}$: tire da raiz os **pares** (ou trios, no caso da raiz cúbica).
$$\sqrt{18x^3} = \sqrt{9 \cdot 2 \cdot x^2 \cdot x} = 3x\sqrt{2x}$$
$$\sqrt{x^7} = \sqrt{x^6 \cdot x} = x^3\sqrt{x}$$

## 4. Racionalização com conjugado

Para tirar a raiz de um denominador do tipo $a + \sqrt{b}$, multiplique em cima e embaixo pelo **conjugado** $a - \sqrt{b}$. A [[Produtos Notáveis#4. Produto da soma pela diferença|diferença de quadrados]] faz a raiz sumir:
$$(a + \sqrt{b})(a - \sqrt{b}) = a^2 - b$$

> [!example] $\dfrac{1}{1 + \sqrt{2}}$
> $$\frac{1}{1 + \sqrt{2}} \cdot \frac{1 - \sqrt{2}}{1 - \sqrt{2}} = \frac{1 - \sqrt{2}}{1 - 2} = \frac{1 - \sqrt{2}}{-1} = \sqrt{2} - 1$$

> [!example] $\dfrac{2}{3 - \sqrt{5}}$
> $$\frac{2(3 + \sqrt{5})}{(3 - \sqrt{5})(3 + \sqrt{5})} = \frac{2(3 + \sqrt{5})}{9 - 5} = \frac{3 + \sqrt{5}}{2}$$

| Denominador | Multiplique por |
|---|---|
| $\sqrt{a}$ | $\sqrt{a}$ |
| $a + \sqrt{b}$ | $a - \sqrt{b}$ |
| $\sqrt{a} - \sqrt{b}$ | $\sqrt{a} + \sqrt{b}$ |

## 5. A forma "soma de potências" (prepare-se para o cálculo)

No cálculo, você vai derivar e integrar termo a termo, e a regra é feita para termos do tipo $a \cdot x^n$. Então é muito útil reescrever:

$$\frac{3x^2 - \sqrt{x}}{x} = \frac{3x^2}{x} - \frac{x^{1/2}}{x} = 3x - x^{-1/2}$$

$$\frac{4}{x^3} - \frac{2}{\sqrt[3]{x}} = 4x^{-3} - 2x^{-1/3}$$

> [!question]- Tente agora (clique para ver as respostas)
> Escreva como soma de potências: (a) $\dfrac{x^3 + 2}{x}$ (b) $x\sqrt{x} + \dfrac{1}{\sqrt{x}}$
> **Respostas:** (a) $x^2 + 2x^{-1}$ (b) $x^{3/2} + x^{-1/2}$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1
> $\dfrac{6a^{-2}b^3}{2a^{-5}b} = 3a^{-2 - (-5)}b^{3 - 1} = 3a^3b^2$

> [!example] Exemplo 2: valor numérico com expoentes fracionários
> Para $x = 4$: $\;x^{3/2} - x^{-1/2} + (0{,}25x)^{-1} = (\sqrt{4})^3 - \frac{1}{\sqrt{4}} + 1^{-1} = 8 - \frac{1}{2} + 1 = \frac{17}{2}$

> [!example] Exemplo 3: quadrado de uma soma com raiz
> $\dfrac{(x + 1)^2}{\sqrt{x}} = (x^2 + 2x + 1) \cdot x^{-1/2} = x^{3/2} + 2x^{1/2} + x^{-1/2}$

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $x^{-1} = -x$ | $\frac{1}{x}$ | o expoente negativo inverte |
| $2x^{-1} = \frac{1}{2x}$ | $\frac{2}{x}$ | o expoente vale só para o $x$ |
| $(x^3)^2 = x^9$ | $x^6$ | potência de potência: **multiplica** |
| $x^2 \cdot x^3 = x^6$ | $x^5$ | produto: **soma** |
| $\sqrt{x^2 + 9} = x + 3$ | não simplifica | a raiz não se distribui na soma |
| $\frac{1}{1 + \sqrt{2}} = 1 + \frac{1}{\sqrt{2}}$ | $\sqrt{2} - 1$ | não se "separa" a soma do denominador |

---

## 💻 Conexão com programação e ML

- ⚠️ `Math.Pow(8, 1/3)` dá **1** em C#! O `1/3` é divisão **inteira** e vale 0, e $8^0 = 1$. O certo é `Math.Pow(8, 1.0/3)`, ou melhor, `Math.Cbrt(8)`.
- **Em ML:**
  - A **regra da potência** do cálculo, $(x^n)' = n x^{n-1}$, só se aplica direto com a expressão na forma $a x^n$. Por isso a seção 5 é tão importante para o [[Cálculo Diferencial]].
  - O **RMSE** é $\left(\frac{1}{n}\sum e_i^2\right)^{1/2}$, e normas $L_p$ são $\left(\sum \lvert x_i \rvert^p\right)^{1/p}$ ([[Produto Escalar e Normas]]).
  - Transformar atributos com $\sqrt{x}$ ou $x^{1/3}$ "achata" valores muito grandes antes de treinar um modelo.

---

## 🔗 Conexões
- **Usa:** [[Potenciação]] e [[Radiciação]] (as mesmas regras), [[Produtos Notáveis]] (o conjugado vem da diferença de quadrados), [[Monômios e Polinômios]].
- **É usado em:** [[Equações do 2º Grau]] (simplificar a raiz de $\Delta$) e [[Equações Redutíveis ao 2º Grau]] (equações irracionais).
- **Mais adiante:** [[Função Exponencial]] (expoentes reais), [[Regras de Derivação]] (regra da potência), [[Integral Indefinida]] e [[Produto Escalar e Normas]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Simplifique $\frac{x^5y^{-2}}{x^{-1}y^3}$ e escreva sem expoentes negativos.
2. Escreva $\frac{1}{\sqrt[3]{x^2}}$ como potência.
3. Por que converter radicais em potências ajuda a multiplicar $\sqrt{x} \cdot \sqrt[4]{x}$?
4. O que é o conjugado de $2 - \sqrt{3}$? Racionalize $\frac{1}{2 - \sqrt{3}}$.
5. Por que $\sqrt{x^2} = \lvert x \rvert$, e não simplesmente $x$?
6. Reescreva $\frac{5x^4 - x}{x^2}$ como soma de potências.
