---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Decimais
  - Dízimas periódicas
  - Fração geratriz
  - Arredondamento
tags:
  - aritmetica
---
# Números Decimais

> [!abstract] Em uma frase
> Os decimais continuam o [[Sistema de Numeração Decimal|sistema posicional]] à direita da vírgula (décimos, centésimos…), e **toda fração** vira um decimal **finito** ou uma **dízima periódica**. O caminho de volta também existe: a **fração geratriz**.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Sistema de Numeração Decimal]], [[Operações com Frações]] · **Próximo:** [[Razão, Proporção e Regra de Três]]
**Praticar:** [[Números Decimais - Exercícios]] · [[Números Decimais - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Converter **decimal ↔ fração** e prever se uma fração dará decimal finito ou dízima.
- Achar a **fração geratriz** de dízimas simples e compostas.
- Fazer as quatro operações com decimais, sem errar a vírgula.
- Arredondar e comparar decimais.

---

## 1. As casas depois da vírgula

$$3{,}725 = 3 + \frac{7}{10} + \frac{2}{100} + \frac{5}{1000}$$

| Unidade | , | Décimo | Centésimo | Milésimo |
|---|---|---|---|---|
| 3 | , | 7 | 2 | 5 |

Cada casa à direita vale $\frac{1}{10}$ da casa anterior. Por isso, multiplicar por 10 **anda a vírgula uma casa para a direita**, e dividir por 10 anda uma casa para a esquerda: $3{,}725 \cdot 100 = 372{,}5$ e $3{,}725 \div 10 = 0{,}3725$.

## 2. Decimal → fração

Leia o número em voz alta e escreva: "setenta e cinco **centésimos**" $= \frac{75}{100} = \frac{3}{4}$.

$$0{,}125 = \frac{125}{1000} = \frac{1}{8} \qquad 2{,}4 = \frac{24}{10} = \frac{12}{5}$$

## 3. Fração → decimal

Divida o numerador pelo denominador: $\frac{3}{8} = 3 \div 8 = 0{,}375$.

> [!tip] Vai dar decimal finito ou dízima?
> Simplifique a fração e fatore o denominador:
> - se ele tem **só os primos 2 e/ou 5**, o decimal é **finito** ($\frac{3}{40}$, com $40 = 2^3 \cdot 5$, dá $0{,}075$);
> - se aparece **qualquer outro primo**, o resultado é uma **dízima periódica** ($\frac{5}{12}$, com $12 = 2^2 \cdot 3$, dá $0{,}41666\dots$).
>
> O motivo: um decimal finito é uma fração com denominador 10, 100, 1000…, e $10 = 2 \cdot 5$.

**Dízimas periódicas:** a parte que se repete é o **período**.
- **Simples:** o período começa logo depois da vírgula. $\frac{1}{3} = 0{,}333\dots = 0{,}\overline{3}$ e $\frac{2}{11} = 0{,}\overline{18}$.
- **Compostas:** há uma parte que não se repete (o **anteperíodo**) antes do período. $\frac{1}{6} = 0{,}1\overline{6} = 0{,}1666\dots$

## 4. Dízima → fração (a fração geratriz)

A ideia é usar multiplicações por 10 para "alinhar" a parte que se repete e depois subtrair, para ela sumir.

> [!example] Simples: $0{,}\overline{18}$
> $$\begin{aligned} x &= 0{,}181818\dots \\ 100x &= 18{,}181818\dots \\ 100x - x &= 18 \\ 99x &= 18 \Rightarrow x = \tfrac{18}{99} = \tfrac{2}{11} \end{aligned}$$

> [!example] Composta: $0{,}1\overline{6}$
> $$\begin{aligned} 10x &= 1{,}666\dots \\ 100x &= 16{,}666\dots \\ 100x - 10x &= 15 \\ 90x &= 15 \Rightarrow x = \tfrac{15}{90} = \tfrac{1}{6} \end{aligned}$$

> [!tip] Regra prática (confira sempre com a divisão)
> - **Simples:** o período sobre tantos **9** quantos forem os algarismos do período: $0{,}\overline{7} = \frac{7}{9}$ e $0{,}\overline{27} = \frac{27}{99} = \frac{3}{11}$.
> - **Composta:** (anteperíodo seguido do período, **menos** o anteperíodo) sobre (um **9** para cada algarismo do período, seguido de um **0** para cada algarismo do anteperíodo): $0{,}1\overline{6} = \frac{16 - 1}{90} = \frac{15}{90} = \frac{1}{6}$.
> - Com parte inteira, separe: $1{,}\overline{3} = 1 + \frac{3}{9} = \frac{4}{3}$.

> [!info] $0{,}999\dots = 1$ (exatamente)
> Pela regra, $0{,}\overline{9} = \frac{9}{9} = 1$. Outro jeito de ver: $\frac{1}{3} = 0{,}333\dots$; multiplicando por 3, $1 = 0{,}999\dots$ Não é "quase 1": é **o mesmo número**, escrito de outro jeito. Isso é uma porta de entrada para a ideia de [[Noção de Limite|limite]].

## 5. Operações

| Operação | Como fazer | Exemplo |
|---|---|---|
| **Soma e subtração** | alinhe as **vírgulas** (complete com zeros) | $3{,}70 + 0{,}48 = 4{,}18$ |
| **Multiplicação** | multiplique como se fossem inteiros; o resultado tem **tantas casas quanto a soma das casas** dos fatores | $0{,}2 \cdot 0{,}3$: $2 \cdot 3 = 6$, 2 casas → $0{,}06$ |
| **Divisão** | multiplique dividendo e divisor pela mesma potência de 10 até o **divisor** virar inteiro | $1{,}2 \div 0{,}04 = 120 \div 4 = 30$ |

> [!tip] Na dúvida, transforme em fração
> $0{,}2 \cdot 0{,}3 = \frac{2}{10} \cdot \frac{3}{10} = \frac{6}{100} = 0{,}06$. E dízimas **sempre** devem virar fração antes de qualquer conta.

## 6. Comparar e arredondar

- **Comparar:** iguale o número de casas. $0{,}5 = 0{,}50 > 0{,}45$.
- **Arredondar** para $n$ casas: olhe a casa seguinte. Se ela for **5 ou mais**, aumente a última casa mantida em uma unidade; se for menor que 5, mantenha. $3{,}14159 \to 3{,}14$ e $7{,}8951 \to 7{,}90$.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: misturando representações
> $0{,}\overline{3} + \frac{1}{6} - 0{,}5 = \frac{1}{3} + \frac{1}{6} - \frac{1}{2} = \frac{2}{6} + \frac{1}{6} - \frac{3}{6} = 0$

> [!example] Exemplo 2: divisão por decimal
> $7{,}5 \div 0{,}25 = 750 \div 25 = 30$ (as duas vírgulas andaram duas casas)

> [!example] Exemplo 3: geratriz com parte inteira
> $2{,}0\overline{45}$: parte inteira 2, anteperíodo 0, período 45. Então $0{,}0\overline{45} = \frac{045 - 0}{990} = \frac{45}{990} = \frac{1}{22}$ e o número é $2 + \frac{1}{22} = \frac{45}{22}$.

> [!example] Exemplo 4: dinheiro
> Gasolina a R\$ 6,29 o litro; 42,5 litros custam $6{,}29 \cdot 42{,}5 = 267{,}325 \approx$ **R\$ 267,33**.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $0{,}45 > 0{,}5$ ("45 é maior que 5") | $0{,}45 < 0{,}50$ | compare casa a casa, com o mesmo número de casas |
| $0{,}2 \cdot 0{,}3 = 0{,}6$ | $0{,}06$ | 1 casa + 1 casa = 2 casas |
| $\frac{1}{3} = 0{,}3$ | $0{,}333\dots$ | $0{,}3 = \frac{3}{10}$, que é outro número |
| $0{,}\overline{18} = \frac{18}{100}$ | $\frac{18}{99}$ | dízima não é decimal finito |
| $0{,}999\dots < 1$ | $= 1$ | |

---

## 💻 Conexão com programação e ML

- **`0.1 + 0.2 == 0.3` é `false` em C#.** O `double` guarda números em **base 2**, e $\frac{1}{10}$ é uma **dízima periódica em binário** ($0{,}0\overline{0011}_2$), assim como $\frac{1}{3}$ é dízima em base 10. O computador corta a dízima e surge um erro minúsculo: `0.30000000000000004`.
- Para dinheiro, use `decimal`, que trabalha em base 10: `0.1m + 0.2m == 0.3m` é `true`.
- Para comparar `double`, use uma tolerância: `Math.Abs(a - b) < 1e-9`.
- ⚠️ `Math.Round(2.5)` dá **2** em C#: o padrão é o "arredondamento bancário" (empate vai para o par). Para o arredondamento da escola, use `Math.Round(2.5, MidpointRounding.AwayFromZero)`, que dá 3.
- **Em ML:** modelos rodam em `float32`, `float16` e até `bfloat16`. Menos bits significam mais erro de arredondamento, mas também mais velocidade e menos memória. Entender que "decimal no computador é aproximado" evita muita surpresa ao comparar resultados.

---

## 🔗 Conexões
- **Usa:** [[Sistema de Numeração Decimal]] (as casas decimais), [[Frações e Equivalência]] e [[Operações com Frações]], [[Múltiplos, Divisores e Primos]] (fatorar o denominador).
- **É usado em:** [[Porcentagem]] (0,15 = 15%), [[Potenciação]] (potências de 10 negativas e notação científica), [[Radiciação]] (raízes decimais), [[Conjuntos Numéricos]] (racionais × irracionais).
- **Mais adiante:** uma dízima é uma soma infinita ($0{,}\overline{3} = 0{,}3 + 0{,}03 + 0{,}003 + \dots$), assunto de [[Séries Geométricas Infinitas]], e $0{,}999\dots = 1$ é um primeiro contato com [[Noção de Limite]].
- **Treino:** [[Treino Misto de Aritmética]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Sem dividir, como saber se $\frac{7}{30}$ dá decimal finito ou dízima?
2. Mostre, com o método de multiplicar por 10, que $0{,}\overline{4} = \frac{4}{9}$.
3. Qual é a fração geratriz de $0{,}2\overline{3}$?
4. Quantas casas decimais tem $1{,}25 \cdot 0{,}004$? Calcule.
5. Como se faz $3{,}6 \div 0{,}12$?
6. Por que `0.1 + 0.2 != 0.3` no computador?
