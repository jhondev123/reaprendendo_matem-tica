---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - MMC
  - MDC
  - Mínimo múltiplo comum
  - Máximo divisor comum
  - Algoritmo de Euclides
tags:
  - aritmetica
---
# MMC e MDC

> [!abstract] Em uma frase
> O **MMC** responde "quando os ciclos coincidem de novo?" e o **MDC** responde "qual o maior pedaço igual que divide tudo sem sobra?". Os dois saem direto da **fatoração em primos**.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Múltiplos, Divisores e Primos]] · **Próximo:** [[Frações e Equivalência]]
**Praticar:** [[MMC e MDC - Exercícios]] · [[MMC e MDC - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Calcular MMC e MDC **por fatoração** e o MDC pelo **algoritmo de Euclides**.
- Saber, pelo enunciado, **qual dos dois** um problema pede.
- Usar a relação $\text{mmc}(a,b) \cdot \text{mdc}(a,b) = a \cdot b$.

---

## 1. Intuição

**MMC (mínimo múltiplo comum):** um ônibus passa a cada 12 min e outro a cada 18 min. Se passaram juntos agora, quando passam juntos de novo?
- Múltiplos de 12: 12, 24, **36**, 48, 60, **72**…
- Múltiplos de 18: 18, **36**, 54, **72**…
- O primeiro em comum é **36**: daqui a 36 minutos.

**MDC (máximo divisor comum):** duas fitas, de 60 cm e 84 cm, serão cortadas em pedaços **iguais**, do **maior tamanho possível**, sem sobra.
- Divisores de 60: 1, 2, 3, 4, 5, 6, 10, **12**, 15, 20, 30, 60
- Divisores de 84: 1, 2, 3, 4, 6, 7, **12**, 14, 21, 28, 42, 84
- O maior em comum é **12 cm**: são $5 + 7 = 12$ pedaços.

> [!tip] Qual usar?
> | O enunciado fala em… | Use |
> |---|---|
> | "juntos de novo", "próximo encontro", "menor quantidade que dá para dividir por todos", "denominador comum" | **MMC** (o resultado é **maior ou igual** aos números) |
> | "maior tamanho possível", "partes iguais sem sobra", "maior número de grupos iguais", "simplificar" | **MDC** (o resultado é **menor ou igual** aos números) |

## 2. Pela fatoração (o método principal)

$$12 = 2^2 \cdot 3 \qquad 18 = 2 \cdot 3^2$$

- **MMC:** **todos** os primos que aparecem, cada um com o **maior** expoente: $\;2^2 \cdot 3^2 = 36$
- **MDC:** só os primos **comuns**, cada um com o **menor** expoente: $\;2^1 \cdot 3^1 = 6$

> [!question]- Por que funciona? (clique para abrir)
> Um múltiplo de 12 precisa "conter" $2^2 \cdot 3$; um múltiplo de 18 precisa conter $2 \cdot 3^2$. Para ser múltiplo dos dois, precisa conter $2^2$ **e** $3^2$, e o menor número assim é $2^2 \cdot 3^2$.
> Já um divisor dos dois só pode usar o que **ambos** têm: no máximo um 2 e um 3.

**Fatoração simultânea** (prática para o MMC de vários números): divida todos juntos pelo menor primo possível, enquanto algum ainda for divisível.

| 12, 18, 30 | 2 |
|---|---|
| 6, 9, 15 | 2 |
| 3, 9, 15 | 3 |
| 1, 3, 5 | 3 |
| 1, 1, 5 | 5 |
| 1, 1, 1 | $\text{mmc} = 2^2 \cdot 3^2 \cdot 5 = 180$ |

## 3. Algoritmo de Euclides (o MDC rápido)

**Ideia:** um divisor comum de $a$ e $b$ também divide o resto de $a \div b$. Então $\text{mdc}(a, b) = \text{mdc}(b, \text{resto})$. Repita até o resto dar zero.

$$\begin{aligned}
252 &= 198 \cdot 1 + 54 \\
198 &= 54 \cdot 3 + 36 \\
54 &= 36 \cdot 1 + \mathbf{18} \\
36 &= 18 \cdot 2 + 0 \quad \Rightarrow \quad \text{mdc}(252, 198) = 18
\end{aligned}$$

O último resto **diferente de zero** é o MDC. É ótimo para números grandes, que são difíceis de fatorar.

## 4. Propriedades úteis

- **Primos entre si:** $\text{mdc}(a, b) = 1$. Por exemplo, 8 e 15. Nesse caso, $\text{mmc}(a, b) = a \cdot b$.
- **Relação de ouro** (para dois números):
$$\text{mmc}(a, b) \cdot \text{mdc}(a, b) = a \cdot b$$
Conferindo: $36 \cdot 6 = 216 = 12 \cdot 18$. ✔️
- Se $a$ divide $b$: $\text{mdc}(a, b) = a$ e $\text{mmc}(a, b) = b$. Por exemplo, mdc(5, 20) = 5 e mmc(5, 20) = 20.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1
> $\text{mdc}(36, 60, 84)$: $\;36 = 2^2 \cdot 3^2$, $\;60 = 2^2 \cdot 3 \cdot 5$, $\;84 = 2^2 \cdot 3 \cdot 7$.
> Comuns com o menor expoente: $2^2 \cdot 3 = 12$.

> [!example] Exemplo 2: luzes
> Três luzes piscam a cada 4, 6 e 10 segundos e acabaram de piscar juntas. Quando piscam juntas de novo?
> $\text{mmc}(4, 6, 10) = 2^2 \cdot 3 \cdot 5 = 60$ s, ou seja, **1 minuto**.

> [!example] Exemplo 3: grupos
> Uma turma tem 24 meninas e 36 meninos. Queremos o **maior número de grupos** com a mesma composição, sem sobrar ninguém.
> $\text{mdc}(24, 36) = 12$ grupos, cada um com $24 \div 12 = 2$ meninas e $36 \div 12 = 3$ meninos.

> [!example] Exemplo 4: usando a relação
> Dois números têm $\text{mmc} = 60$ e $\text{mdc} = 4$. Um deles é 12. Qual é o outro?
> $60 \cdot 4 = 12 \cdot b \Rightarrow b = \frac{240}{12} = 20$.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| Achar o MMC como o produto: $\text{mmc}(12, 18) = 216$ | $36$ | o produto é **um** múltiplo comum, não o menor (só coincide quando são primos entre si) |
| MMC: usar o **menor** expoente | MMC: o **maior**; MDC: o **menor** | |
| MDC com primos **não** comuns | só os comuns | um divisor dos dois só pode usar o que os dois têm |
| Usar MMC num problema de "maior pedaço" | MDC | releia a tabela "Qual usar?" |
| A relação mmc · mdc = produto para 3 números | vale só para **dois** | |

---

## 💻 Conexão com programação e ML

- **Euclides em uma linha:** `int Mdc(int a, int b) => b == 0 ? a : Mdc(b, a % b);`. É um dos algoritmos mais antigos que ainda se usam. Para números enormes, o .NET tem `BigInteger.GreatestCommonDivisor`.
- **MMC a partir do MDC:** `a / Mdc(a, b) * b` (dividir antes de multiplicar evita *overflow*).
- **Proporção de tela:** $\text{mdc}(1920, 1080) = 120$, e $1920 \div 120 = 16$, $1080 \div 120 = 9$: a tela é **16:9**.
- **Em ML e ciência de dados:** ao combinar séries temporais com frequências diferentes (dados de hora em hora com dados a cada 15 minutos), o "passo comum" é um MMC/MDC de períodos. E simplificar razões é o primeiro passo de [[Frações e Equivalência]].

---

## 🔗 Conexões
- **Usa:** [[Múltiplos, Divisores e Primos]] (fatoração), [[Operações Fundamentais]] (o resto, no algoritmo de Euclides).
- **É usado em:**
  - [[Frações e Equivalência]]: simplificar uma fração é dividir pelo **MDC**.
  - [[Operações com Frações]]: somar frações pede o **MMC** dos denominadores.
- **Na álgebra:** [[Frações Algébricas]] usam o MMC de **polinômios**, com a mesma regra dos maiores expoentes.
- **Mais adiante:** o período de uma soma de funções periódicas é um MMC ([[Funções Seno e Cosseno]]).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Em palavras, o que é o MMC? E o MDC? Dê um exemplo de problema para cada.
2. Como achar MMC e MDC pela fatoração? Qual usa o maior expoente?
3. Calcule $\text{mdc}(84, 30)$ pelo algoritmo de Euclides.
4. O que significa dois números serem primos entre si? Quanto vale o MMC deles?
5. Escreva a relação entre MMC, MDC e o produto de dois números.
6. Por que o MMC é sempre maior ou igual aos números, e o MDC, menor ou igual?
