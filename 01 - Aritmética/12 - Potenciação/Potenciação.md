---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Potências
  - Expoente
  - Notação científica
  - Propriedades das potências
tags:
  - aritmetica
---
# Potenciação

> [!abstract] Em uma frase
> $a^n$ é a multiplicação de $a$ por ele mesmo $n$ vezes. Todas as propriedades (inclusive $a^0 = 1$ e $a^{-n} = \frac{1}{a^n}$) saem de uma só ideia: **multiplicar potências de mesma base é somar expoentes**.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Números Inteiros]], [[Operações com Frações]], [[Números Decimais]] · **Próximo:** [[Radiciação]]
**Praticar:** [[Potenciação - Exercícios]] · [[Potenciação - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Calcular potências com base inteira, negativa, fracionária e decimal.
- Explicar **por que** $a^0 = 1$ e $a^{-n} = \frac{1}{a^n}$.
- Usar as **cinco propriedades** para simplificar expressões.
- Escrever e operar números em **notação científica**.

---

## 1. Definição

$$a^n = \underbrace{a \cdot a \cdot a \cdots a}_{n \text{ fatores}} \qquad 2^5 = 2 \cdot 2 \cdot 2 \cdot 2 \cdot 2 = 32$$

$a$ é a **base**, $n$ é o **expoente** e o resultado é a **potência**. $a^2$ se lê "a ao quadrado" (a área de um quadrado de lado $a$); $a^3$, "a ao cubo" (o volume de um cubo de aresta $a$).

> [!tip] Decore estas (elas aparecem o tempo todo)
> | $n$ | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
> |---|---|---|---|---|---|---|---|---|---|---|
> | $2^n$ | 2 | 4 | 8 | 16 | 32 | 64 | 128 | 256 | 512 | 1024 |
> | $3^n$ | 3 | 9 | 27 | 81 | 243 | | | | | |
> | $n^2$ | 1 | 4 | 9 | 16 | 25 | 36 | 49 | 64 | 81 | 100 |
>
> E também $11^2 = 121$, $12^2 = 144$, $13^2 = 169$, $14^2 = 196$, $15^2 = 225$.

## 2. Sinais e bases especiais

| Caso | Regra | Exemplo |
|---|---|---|
| Base negativa, expoente **par** | resultado positivo | $(-2)^4 = 16$ |
| Base negativa, expoente **ímpar** | resultado negativo | $(-2)^3 = -8$ |
| **Sem parênteses** | o expoente não "pega" o sinal | $-2^4 = -16$ |
| Base fracionária | eleve o numerador e o denominador | $\left(\frac{2}{3}\right)^3 = \frac{8}{27}$ |
| Base decimal | a quantidade de casas se multiplica | $0{,}2^3 = 0{,}008$ (3 casas) |
| Base 1 ou 0 | $1^n = 1$; $0^n = 0$ (para $n > 0$) | $1^{100} = 1$ |

## 3. As propriedades (todas vêm da definição)

| Propriedade | Fórmula | Por quê | Exemplo |
|---|---|---|---|
| **Produto de mesma base** | $a^m \cdot a^n = a^{m+n}$ | juntam-se $m$ fatores com mais $n$ fatores | $2^3 \cdot 2^5 = 2^8$ |
| **Quociente de mesma base** | $\dfrac{a^m}{a^n} = a^{m-n}$ | $n$ fatores se cancelam | $\frac{5^7}{5^4} = 5^3$ |
| **Potência de potência** | $(a^m)^n = a^{m \cdot n}$ | $n$ grupos de $m$ fatores | $(3^2)^4 = 3^8$ |
| **Potência de produto** | $(a \cdot b)^n = a^n \cdot b^n$ | reorganizando os fatores | $(2 \cdot 5)^3 = 2^3 \cdot 5^3$ |
| **Potência de quociente** | $\left(\dfrac{a}{b}\right)^n = \dfrac{a^n}{b^n}$ | idem | $\left(\frac{3}{4}\right)^2 = \frac{9}{16}$ |

> [!danger] O que **não** é propriedade
> - $(a + b)^n \neq a^n + b^n$: por exemplo, $(2 + 3)^2 = 25$, mas $2^2 + 3^2 = 13$. (Veja [[Produtos Notáveis]].)
> - $a^m + a^n \neq a^{m+n}$: $2^3 + 2^2 = 12$, mas $2^5 = 32$.
> - $2^3 \neq 2 \cdot 3$: $2^3 = 8$.

## 4. Expoente zero e expoente negativo

Use a propriedade do quociente com expoentes iguais: $\frac{a^3}{a^3} = a^{3-3} = a^0$. Mas qualquer número (diferente de zero) dividido por ele mesmo é 1. Então:

$$a^0 = 1 \quad (a \neq 0)$$

E se o expoente de baixo for maior? $\frac{a^2}{a^5} = a^{2-5} = a^{-3}$. Cancelando os fatores, a mesma fração dá $\frac{1}{a^3}$. Então:

$$a^{-n} = \frac{1}{a^n} \qquad \left(\frac{a}{b}\right)^{-n} = \left(\frac{b}{a}\right)^{n}$$

> [!example] Veja o padrão
> $$2^3 = 8 \;\xrightarrow{\div 2}\; 2^2 = 4 \;\xrightarrow{\div 2}\; 2^1 = 2 \;\xrightarrow{\div 2}\; 2^0 = 1 \;\xrightarrow{\div 2}\; 2^{-1} = \tfrac{1}{2} \;\xrightarrow{\div 2}\; 2^{-2} = \tfrac{1}{4}$$
> Cada passo para a direita divide por 2. Nada de mágica: é só continuar o padrão.

**O expoente negativo não deixa o número negativo**: ele **inverte**. $2^{-3} = \frac{1}{8}$, e não $-8$.

## 5. Potências de 10

$$10^3 = 1000 \qquad 10^0 = 1 \qquad 10^{-1} = 0{,}1 \qquad 10^{-3} = 0{,}001$$

Expoente positivo: é a quantidade de **zeros**. Expoente negativo: é a quantidade de **casas decimais**.

## 6. Notação científica

Um número em notação científica tem a forma
$$a \times 10^n, \qquad \text{com } 1 \leq a < 10 \text{ e } n \text{ inteiro}$$

| Número | Notação científica |
|---|---|
| Velocidade da luz: 300.000.000 m/s | $3 \times 10^8$ m/s |
| 45.000.000 | $4{,}5 \times 10^7$ |
| 0,00032 | $3{,}2 \times 10^{-4}$ |

**Regra prática:** ande com a vírgula até sobrar um único algarismo (diferente de zero) antes dela. Cada casa andada para a **esquerda** soma 1 ao expoente; cada casa para a **direita** subtrai 1.

**Operações:** multiplique ou divida as partes "$a$" e use as propriedades nas potências de 10:
$$(3 \times 10^8) \cdot (2 \times 10^{-3}) = 6 \times 10^{5} \qquad \frac{8 \times 10^6}{4 \times 10^{-2}} = 2 \times 10^{8}$$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: simplificar
> $$\frac{2^5 \cdot 2^{-2}}{2^4} = \frac{2^{3}}{2^4} = 2^{-1} = \frac{1}{2}$$

> [!example] Exemplo 2: mesma base escondida
> $8^3 \cdot 4^2 = (2^3)^3 \cdot (2^2)^2 = 2^9 \cdot 2^4 = 2^{13}$

> [!example] Exemplo 3: misturando tudo
> $$(-2)^3 + \left(\tfrac{1}{2}\right)^{-2} - 3^0 + 0{,}5^2 = -8 + 4 - 1 + 0{,}25 = -4{,}75$$

> [!example] Exemplo 4: comparar
> Qual é maior, $2^{30}$ ou $10^9$? Como $2^{30} = (2^{10})^3 = 1024^3$ e $10^9 = 1000^3$, o maior é $2^{30}$.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $2^3 = 6$ | $8$ | é multiplicação repetida, não base vezes expoente |
| $2^{-3} = -8$ | $\frac{1}{8}$ | o expoente negativo inverte |
| $-3^2 = 9$ | $-9$ | sem parênteses, o expoente vale só para o 3 |
| $2^3 \cdot 2^4 = 2^{12}$ | $2^7$ | no produto, **somam-se** os expoentes |
| $2^3 \cdot 3^2 = 6^5$ | $8 \cdot 9 = 72$ | as propriedades exigem **mesma base** (ou mesmo expoente) |
| $(2+3)^2 = 4 + 9$ | $25$ | a potência não se distribui na soma |
| $5^0 = 0$ | $1$ | |

---

## 💻 Conexão com programação e ML

- `Math.Pow(2, 10)` devolve `1024.0` (um `double`). Para inteiros, `1 << n` é $2^n$, e é muito mais rápido.
- **Notação científica no código:** `1e-3` é $1 \times 10^{-3} = 0{,}001$ e `6.02e23` é $6{,}02 \times 10^{23}$.
- $2^{10} = 1024 \approx 10^3$: por isso 1 KiB = 1024 bytes, enquanto 1 KB = 1000 bytes. Um `int` vai até $2^{31} - 1 \approx 2{,}1 \times 10^9$.
- **Em ML:**
  - Taxas de aprendizado como `3e-4`, regularização `1e-5`, tolerâncias `1e-8`: é tudo notação científica.
  - "Um modelo de 7B" tem $7 \times 10^9$ parâmetros. A 2 bytes cada, são $1{,}4 \times 10^{10}$ bytes, ou seja, cerca de 14 GB de memória só para os pesos.
  - O **erro quadrático** eleva cada erro ao quadrado, e o [[Função Exponencial|crescimento exponencial]] aparece na função *softmax* ($e^x$).

---

## 🔗 Conexões
- **Usa:** [[Números Inteiros]] (sinais), [[Operações com Frações]] (bases fracionárias e expoente negativo), [[Números Decimais]] e [[Sistema de Numeração Decimal]] (potências de 10).
- **É usado em:**
  - [[Radiciação]]: a raiz é a operação inversa da potência, e $\sqrt{a} = a^{1/2}$.
  - [[Múltiplos, Divisores e Primos]]: na fatoração, $360 = 2^3 \cdot 3^2 \cdot 5$.
  - [[Porcentagem]]: nos juros compostos, $(1 + i)^t$.
- **Na álgebra:** [[Monômios e Polinômios]] ($x^2 \cdot x^3 = x^5$) e [[Expoentes e Radicais com Variáveis]] (as mesmas propriedades, com letras).
- **Mais adiante:** [[Função Exponencial]], [[Definição de Logaritmo]] (o logaritmo é "o expoente"), [[Progressão Geométrica]].
- **Treino:** [[Treino Misto de Aritmética]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Enuncie as cinco propriedades das potências.
2. Use uma propriedade para mostrar que $7^0 = 1$.
3. Quanto vale $\left(\frac{2}{5}\right)^{-2}$? Por quê?
4. Qual é a diferença entre $(-5)^2$ e $-5^2$?
5. Escreva 0,000072 e 830.000 em notação científica.
6. Por que $(a + b)^2 \neq a^2 + b^2$? Dê um contraexemplo.
