---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Somatório
  - Notação sigma
  - Produtório
  - Sigma
tags:
  - algebra
---
# Somatório e Produtório

> [!abstract] Em uma frase
> $\sum_{i=1}^{n} x_i$ é um **laço `for` escrito em matemática**: "some $x_i$ para $i$ indo de 1 até $n$". É **a** notação das fórmulas de estatística e machine learning, e o $\prod$ faz o mesmo com multiplicações.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Linguagem Algébrica]], [[Operações Fundamentais]] · **Próximo:** [[Funções]] (próximo tema)
**Praticar:** [[Somatório e Produtório - Exercícios]] · [[Somatório e Produtório - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- **Ler e escrever** somatórios e produtórios.
- Calcular somatórios usando as **propriedades** (linearidade) e a soma de Gauss.
- Saber o que **não** se pode fazer: $\sum x_i^2 \neq \left(\sum x_i\right)^2$.
- Ler as fórmulas de **média**, **erro quadrático médio** e **produto escalar**.

---

## 1. A anatomia

$$\sum_{i=1}^{n} x_i = x_1 + x_2 + x_3 + \dots + x_n$$

| Parte | Nome | No código |
|---|---|---|
| $\Sigma$ | sigma maiúsculo: "some" | `soma +=` |
| $i$ | **índice** (a variável do laço) | `int i` |
| $i = 1$ | limite inferior (onde começa) | `i = 1` |
| $n$ | limite superior (onde termina, **incluído**) | `i <= n` |
| $x_i$ | o **termo geral** | `x[i]` |

```csharp
double soma = 0;
for (int i = 1; i <= n; i++)
    soma += x[i];
```

> [!example] Abrindo somatórios
> - $\sum_{i=1}^{5} i = 1 + 2 + 3 + 4 + 5 = 15$
> - $\sum_{k=1}^{4} k^2 = 1 + 4 + 9 + 16 = 30$
> - $\sum_{i=1}^{3} (2i + 1) = 3 + 5 + 7 = 15$
> - $\sum_{i=1}^{10} 7 = \underbrace{7 + 7 + \dots + 7}_{10 \text{ vezes}} = 70$

> [!tip] Detalhes importantes
> - **Número de termos:** de $i = a$ até $i = b$, são $b - a + 1$ termos (como em [[Sistema de Numeração Decimal]]: de 100 a 999 são 900 números).
> - **O nome do índice não importa:** $\sum_{i=1}^{n} x_i = \sum_{k=1}^{n} x_k$, assim como renomear a variável do `for` não muda o resultado.
> - **Constante:** $\sum_{i=1}^{n} c = n \cdot c$ (e **não** $c$).

## 2. Propriedades (a "linearidade")

| Propriedade | Fórmula | Em palavras |
|---|---|---|
| Soma separa | $\sum (a_i + b_i) = \sum a_i + \sum b_i$ | dá para somar em duas etapas |
| Constante sai | $\sum c \cdot a_i = c \sum a_i$ | é a [[Operações Fundamentais#3. Propriedades\|distributiva]]: $ca_1 + ca_2 = c(a_1 + a_2)$ |
| Constante sozinha | $\sum_{i=1}^{n} c = nc$ | |

> [!danger] O que NÃO vale
> $$\sum a_i b_i \neq \left(\sum a_i\right)\left(\sum b_i\right) \qquad \sum x_i^2 \neq \left(\sum x_i\right)^2$$
> Teste com $x = (1, 2)$: $\sum x_i^2 = 1 + 4 = 5$, mas $\left(\sum x_i\right)^2 = 3^2 = 9$. É o mesmo erro de $(a + b)^2 \neq a^2 + b^2$ ([[Produtos Notáveis]]).

## 3. Somas que vale saber

$$\sum_{i=1}^{n} i = \frac{n(n + 1)}{2}$$
É a soma de Gauss, que você calculou nos exercícios de [[Operações Fundamentais - Exercícios|Operações Fundamentais]].

$$\sum_{i=1}^{n} (2i - 1) = n^2$$
É a soma dos $n$ primeiros ímpares.

E a **soma telescópica** de [[Operações com Frações]]: $\sum_{k=1}^{n} \frac{1}{k(k+1)} = 1 - \frac{1}{n + 1}$.

## 4. Produtório

$$\prod_{i=1}^{n} x_i = x_1 \cdot x_2 \cdots x_n$$

- $\prod_{i=1}^{4} i = 1 \cdot 2 \cdot 3 \cdot 4 = 24 = 4!$ (o **fatorial**, de [[Fatorial e Permutações]])
- $\prod_{i=1}^{3} 2 = 2^3 = 8$, ou seja, $\prod_{i=1}^{n} c = c^n$

> [!info] O logaritmo transforma produto em soma
> Em [[Propriedades dos Logaritmos]] você vai ver que $\log(ab) = \log a + \log b$. Então $\log \prod x_i = \sum \log x_i$. Esse truque é usado o tempo todo em ML (veja abaixo).

## 5. Somatório duplo

$\sum_{i=1}^{2} \sum_{j=1}^{3} (i + j)$ é um **laço dentro de outro**: para cada $i$, percorre todos os $j$.
$$= \underbrace{(2 + 3 + 4)}_{i = 1} + \underbrace{(3 + 4 + 5)}_{i = 2} = 9 + 12 = 21$$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: usando as propriedades
> Se $\sum_{i=1}^{20} a_i = 50$ e $\sum_{i=1}^{20} b_i = 30$, então
> $$\sum_{i=1}^{20} (3a_i - 2b_i + 1) = 3 \cdot 50 - 2 \cdot 30 + 20 \cdot 1 = 150 - 60 + 20 = 110$$

> [!example] Exemplo 2: média
> A **média** de $n$ valores é $\bar{x} = \frac{1}{n}\sum_{i=1}^{n} x_i$. Para $x = (2, 5, 3, 8, 7)$: $\bar{x} = \frac{25}{5} = 5$.

> [!example] Exemplo 3: com frações
> $\sum_{k=1}^{4} \left(\frac{1}{2}\right)^k = \frac{1}{2} + \frac{1}{4} + \frac{1}{8} + \frac{1}{16} = \frac{15}{16}$ (cada vez mais perto de 1; veja [[Séries Geométricas Infinitas]]).

> [!example] Exemplo 4: sinais alternados
> $\sum_{i=1}^{4} (-1)^i \cdot i = -1 + 2 - 3 + 4 = 2$

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $\sum_{i=1}^{10} 5 = 5$ | $50$ | são 10 parcelas iguais a 5 |
| $\sum_{i=3}^{12}$ tem 9 termos | 10 termos | $12 - 3 + 1$ |
| $\sum x_i^2 = \left(\sum x_i\right)^2$ | são diferentes | elevar ao quadrado antes ou depois de somar muda tudo |
| Tirar para fora algo que depende de $i$: $\sum i \cdot x_i = i \sum x_i$ | não pode | só sai o que é **constante** em relação ao índice |

---

## 💻 Conexão com programação e ML

**No código**, somatório e produtório são `Sum` e `Aggregate`:
```csharp
int s = Enumerable.Range(1, 5).Sum();                    // Σ i = 15
int q = Enumerable.Range(1, 4).Sum(k => k * k);          // Σ k² = 30
long p = Enumerable.Range(1, 4).Aggregate(1L, (a, i) => a * i); // Π i = 24
```

**Em ML, praticamente toda fórmula tem um $\Sigma$.** Agora você consegue lê-las:

| Fórmula | Nome | O que faz |
|---|---|---|
| $\bar{x} = \frac{1}{n}\sum_{i=1}^{n} x_i$ | média | soma tudo e divide pela quantidade |
| $\text{MSE} = \frac{1}{n}\sum_{i=1}^{n} (y_i - \hat{y}_i)^2$ | erro quadrático médio | média dos erros ao quadrado |
| $\mathbf{w} \cdot \mathbf{x} = \sum_{j=1}^{d} w_j x_j$ | produto escalar | o que cada neurônio calcula (veja [[Produto Escalar e Normas]]) |
| $z = \sum_j w_j x_j + b$ | saída de um neurônio | produto escalar mais o viés |
| $L(\theta) = \prod_{i=1}^{n} p(x_i \mid \theta)$ | verossimilhança | a probabilidade dos dados (veja [[Máxima Verossimilhança]]) |
| $\log L = \sum_{i=1}^{n} \log p(x_i \mid \theta)$ | log-verossimilhança | o mesmo, mas como soma (mais estável) |
| $\text{softmax}(z)_k = \frac{e^{z_k}}{\sum_j e^{z_j}}$ | softmax | transforma pontuações em probabilidades |

> [!tip] Por que a log-verossimilhança?
> Multiplicar milhares de probabilidades pequenas (como 0,01) dá um número tão pequeno que o `double` arredonda para zero (*underflow*). Somar os logaritmos dá o mesmo resultado, sem esse problema. É o $\prod$ virando $\sum$.

---

## 🔗 Conexões
- **Usa:** [[Linguagem Algébrica]] (índices como $x_1, x_2$), [[Operações Fundamentais]] (soma de Gauss e distributiva), [[Operações com Frações]] (somas telescópicas), [[Produtos Notáveis]] (por que $\sum x^2 \neq (\sum x)^2$).
- **Mais adiante:**
  - [[Soma dos Termos de PA e PG]] e [[Séries Geométricas Infinitas]].
  - [[Somas de Riemann]] e [[Integral Definida]]: a integral é um "somatório contínuo" ($\int$ é um S esticado).
  - [[Medidas de Tendência Central]] e [[Medidas de Dispersão]]: média, variância e desvio padrão.
  - [[Produto Escalar e Normas]], [[Máxima Verossimilhança]] e [[Entropia e Cross-Entropy]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Escreva $\sum_{i=2}^{6} (i^2 - 1)$ por extenso e calcule.
2. Transforme $\sum_{i=1}^{n} x_i$ num laço `for` em C#.
3. Quanto vale $\sum_{i=1}^{50} 4$? E $\sum_{i=1}^{50} 4i$?
4. Quais são as propriedades do somatório? Por que $\sum x_i^2 \neq (\sum x_i)^2$?
5. Escreva a fórmula do MSE e explique cada símbolo.
6. Por que se usa $\sum \log p_i$ em vez de $\prod p_i$?
