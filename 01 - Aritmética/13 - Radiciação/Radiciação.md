---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Raiz quadrada
  - Raízes
  - Radicais
  - Expoente fracionário
  - Racionalização
tags:
  - aritmetica
---
# Radiciação

> [!abstract] Em uma frase
> A raiz **desfaz** a potência: $\sqrt[n]{a} = b$ significa $b^n = a$. E toda raiz é uma potência de **expoente fracionário**, $\sqrt[n]{a} = a^{1/n}$, então valem as mesmas propriedades de [[Potenciação]].

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Potenciação]], [[Múltiplos, Divisores e Primos]] · **Próximo:** [[Conjuntos Numéricos]]
**Praticar:** [[Radiciação - Exercícios]] · [[Radiciação - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Calcular raízes exatas e **estimar** raízes não exatas.
- **Simplificar** radicais pela fatoração e operar com eles.
- **Racionalizar** denominadores simples.
- Converter entre raiz e **expoente fracionário**.

---

## 1. Definição

$$\sqrt[n]{a} = b \iff b^n = a$$

$n$ é o **índice**, $a$ é o **radicando** e $b$ é a **raiz**. Quando o índice é 2, ele não se escreve: $\sqrt{a}$.

| Raiz | Porque | |
|---|---|---|
| $\sqrt{81} = 9$ | $9^2 = 81$ | |
| $\sqrt[3]{8} = 2$ | $2^3 = 8$ | |
| $\sqrt[3]{-8} = -2$ | $(-2)^3 = -8$ | índice ímpar aceita radicando negativo |
| $\sqrt{-4}$ | não existe nos reais | nenhum número real ao quadrado dá negativo |
| $\sqrt{\tfrac{4}{9}} = \tfrac{2}{3}$ | $\left(\tfrac{2}{3}\right)^2 = \tfrac{4}{9}$ | |
| $\sqrt{0{,}09} = 0{,}3$ | $0{,}3^2 = 0{,}09$ | |

> [!important] $\sqrt{4} = 2$, e não $\pm 2$
> O símbolo $\sqrt{\phantom{a}}$ indica a raiz **não negativa**. Quem tem duas respostas é a **equação** $x^2 = 4$: $x = 2$ ou $x = -2$, ou seja, $x = \pm\sqrt{4}$. Essa diferença é essencial em [[Equações do 2º Grau]].
> Pelo mesmo motivo, $\sqrt{x^2} = \lvert x \rvert$ (o [[Números Inteiros|módulo]]): $\sqrt{(-3)^2} = \sqrt{9} = 3$.

## 2. Estimando raízes

$\sqrt{50}$: como $7^2 = 49$ e $8^2 = 64$, temos $7 < \sqrt{50} < 8$, bem perto de 7. De fato, $\sqrt{50} \approx 7{,}07$.

Vale decorar: $\sqrt{2} \approx 1{,}414$, $\;\sqrt{3} \approx 1{,}732$, $\;\sqrt{5} \approx 2{,}236$.

## 3. Propriedades

Valem para radicandos não negativos (e também para índices ímpares com radicandos negativos):

| Propriedade | Fórmula | Exemplo |
|---|---|---|
| Raiz do produto | $\sqrt[n]{a \cdot b} = \sqrt[n]{a} \cdot \sqrt[n]{b}$ | $\sqrt{4 \cdot 25} = 2 \cdot 5 = 10$ |
| Raiz do quociente | $\sqrt[n]{\dfrac{a}{b}} = \dfrac{\sqrt[n]{a}}{\sqrt[n]{b}}$ | $\sqrt{\frac{9}{16}} = \frac{3}{4}$ |
| Potência da raiz | $\left(\sqrt[n]{a}\right)^m = \sqrt[n]{a^m}$ | $(\sqrt{5})^2 = 5$ |
| Raiz de raiz | $\sqrt[m]{\sqrt[n]{a}} = \sqrt[m \cdot n]{a}$ | $\sqrt{\sqrt{16}} = \sqrt[4]{16} = 2$ |

> [!danger] A raiz **não** se distribui na soma
> $$\sqrt{a + b} \neq \sqrt{a} + \sqrt{b} \qquad \sqrt{9 + 16} = \sqrt{25} = 5, \text{ mas } \sqrt{9} + \sqrt{16} = 7$$
> É o mesmo erro de $(a + b)^2 \neq a^2 + b^2$, visto em [[Potenciação]].

## 4. Simplificando radicais

Fatore o radicando e "tire" da raiz cada grupo de $n$ fatores iguais:

$$\sqrt{72} = \sqrt{2^3 \cdot 3^2} = \sqrt{2^2 \cdot 3^2 \cdot 2} = 2 \cdot 3 \cdot \sqrt{2} = 6\sqrt{2}$$

$$\sqrt[3]{54} = \sqrt[3]{3^3 \cdot 2} = 3\sqrt[3]{2}$$

Use a fatoração em primos de [[Múltiplos, Divisores e Primos]].

## 5. Operações com radicais

- **Somar e subtrair:** só se juntam **radicais semelhantes** (mesmo índice e mesmo radicando), como se fossem "unidades". $3\sqrt{2} + 5\sqrt{2} = 8\sqrt{2}$. Às vezes é preciso simplificar antes: $\sqrt{8} + \sqrt{18} = 2\sqrt{2} + 3\sqrt{2} = 5\sqrt{2}$.
- **Multiplicar e dividir** (mesmo índice): junte numa raiz só. $\sqrt{3} \cdot \sqrt{12} = \sqrt{36} = 6$ e $\frac{\sqrt{50}}{\sqrt{2}} = \sqrt{25} = 5$.

> [!warning] $\sqrt{2} + \sqrt{3} \neq \sqrt{5}$
> Radicais diferentes **não se somam** (assim como $2x + 3y$ não vira $5xy$). O resultado fica $\sqrt{2} + \sqrt{3} \approx 3{,}15$.

## 6. Racionalização (raiz fora do denominador)

Multiplique o numerador e o denominador pela raiz que está embaixo (é multiplicar por 1):

$$\frac{1}{\sqrt{2}} = \frac{1}{\sqrt{2}} \cdot \frac{\sqrt{2}}{\sqrt{2}} = \frac{\sqrt{2}}{2} \qquad \frac{6}{\sqrt{3}} = \frac{6\sqrt{3}}{3} = 2\sqrt{3}$$

Com binômios no denominador, como $\frac{1}{1 + \sqrt{2}}$, usa-se o **conjugado**. Isso fica para [[Expoentes e Radicais com Variáveis]].

## 7. Expoente fracionário

$$a^{\frac{m}{n}} = \sqrt[n]{a^m} = \left(\sqrt[n]{a}\right)^m$$

O **denominador** do expoente é o índice da raiz; o **numerador** é a potência.

$$8^{\frac{2}{3}} = \left(\sqrt[3]{8}\right)^2 = 2^2 = 4 \qquad 16^{\frac{1}{2}} = 4 \qquad 27^{-\frac{1}{3}} = \frac{1}{\sqrt[3]{27}} = \frac{1}{3}$$

> [!tip] Calcule a raiz primeiro
> Em $8^{2/3}$, é mais fácil fazer $\sqrt[3]{8} = 2$ e depois $2^2 = 4$ do que $8^2 = 64$ e depois $\sqrt[3]{64} = 4$.

Com isso, as propriedades das raízes viram propriedades das potências: $\sqrt{a} \cdot \sqrt{a} = a^{1/2} \cdot a^{1/2} = a^{1} = a$.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1
> $\sqrt{8} + \sqrt{18} - \sqrt{32} = 2\sqrt{2} + 3\sqrt{2} - 4\sqrt{2} = \sqrt{2}$

> [!example] Exemplo 2: misturando conjuntos
> $\sqrt{0{,}\overline{4}} + \sqrt[3]{\tfrac{8}{27}}$. Primeiro, a dízima vira fração: $0{,}\overline{4} = \frac{4}{9}$. Então $\sqrt{\tfrac{4}{9}} + \tfrac{2}{3} = \tfrac{2}{3} + \tfrac{2}{3} = \tfrac{4}{3}$.

> [!example] Exemplo 3: expoentes fracionários
> $27^{2/3} - 16^{-1/2} + 0{,}01^{1/2} = 9 - \frac{1}{4} + 0{,}1 = 8{,}85$

> [!example] Exemplo 4: um quadrado de área 72 cm²
> O lado é $\sqrt{72} = 6\sqrt{2} \approx 6 \cdot 1{,}414 \approx 8{,}49$ cm.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $\sqrt{9 + 16} = 3 + 4$ | $\sqrt{25} = 5$ | a raiz não se distribui na soma |
| $\sqrt{-9} = -3$ | não existe em $\mathbb{R}$ | $(-3)^2 = 9$, e não $-9$ |
| $\sqrt{4} = \pm 2$ | $2$ | o $\pm$ aparece ao **resolver** $x^2 = 4$ |
| $\sqrt{2} + \sqrt{3} = \sqrt{5}$ | fica $\sqrt{2} + \sqrt{3}$ | não são semelhantes |
| $2\sqrt{3} = \sqrt{6}$ | $2\sqrt{3} = \sqrt{12}$ | para "entrar" na raiz, o 2 entra ao quadrado |
| $8^{2/3} = \frac{16}{3}$ | $4$ | o expoente fracionário é uma raiz, não uma multiplicação |

---

## 💻 Conexão com programação e ML

- `Math.Sqrt(-1)` devolve `NaN`. E cuidado: `Math.Pow(-8, 1.0/3)` também dá `NaN`; use `Math.Cbrt(-8)`, que dá `-2`.
- **Método babilônico** (de Newton) para a raiz quadrada: comece com um palpite $x$ e repita $x \leftarrow \frac{x + a/x}{2}$. Converge muito rápido. É um exemplo de método iterativo, como os de otimização em ML, e o método de Newton vem do [[Cálculo Diferencial]].
- **Em ML a raiz está em toda parte:**
  - **Distância euclidiana** entre pontos/vetores: $\sqrt{(x_1 - y_1)^2 + (x_2 - y_2)^2 + \dots}$, base do k-NN e do k-means.
  - **Norma L2** de um vetor ($\lVert v \rVert$) e o **desvio padrão** (a raiz da variância).
  - **RMSE** (a raiz do erro quadrático médio), o otimizador **Adam** (divide pelo $\sqrt{v}$) e a atenção dos Transformers, que divide por $\sqrt{d_k}$.

---

## 🔗 Conexões
- **Usa:** [[Potenciação]] (a raiz é a sua inversa), [[Múltiplos, Divisores e Primos]] (simplificar pela fatoração), [[Números Decimais]] e [[Operações com Frações]] (raízes de decimais e de frações).
- **É usado em:** [[Conjuntos Numéricos]] ($\sqrt{2}$ é irracional).
- **Na álgebra:** [[Expoentes e Radicais com Variáveis]] (racionalização com conjugado), [[Equações do 2º Grau]] (a fórmula de Bhaskara usa $\sqrt{\Delta}$), [[Equações Redutíveis ao 2º Grau]] (equações irracionais).
- **Mais adiante:** [[Teorema de Pitágoras]], [[Distância entre Pontos]], [[Medidas de Dispersão]] (desvio padrão) e [[Produto Escalar e Normas]].
- **Treino:** [[Treino Misto de Aritmética]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. O que significa $\sqrt[3]{-27} = -3$? Por que $\sqrt{-27}$ não existe nos reais?
2. Por que $\sqrt{9} = 3$, mas $x^2 = 9$ tem duas soluções?
3. Simplifique $\sqrt{200}$ e $\sqrt[3]{40}$.
4. Quando se pode somar dois radicais? Calcule $\sqrt{12} + \sqrt{27}$.
5. Racionalize $\frac{5}{\sqrt{5}}$.
6. Escreva $\sqrt[4]{a^3}$ como potência e calcule $32^{3/5}$.
