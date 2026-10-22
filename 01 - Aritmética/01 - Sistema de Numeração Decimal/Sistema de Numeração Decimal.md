---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Valor posicional
  - Base 10
  - Binário
tags:
  - aritmetica
---
# Sistema de Numeração Decimal

> [!abstract] Em uma frase
> No nosso sistema de numeração, **o valor de um algarismo depende da posição em que ele está**, e cada posição vale **10 vezes** a posição à sua direita.

**Tema:** [[Aritmética]] · **Pré-requisitos:** nenhum · **Próximo:** [[Operações Fundamentais]]
**Praticar:** [[Sistema de Numeração Decimal - Exercícios]] · [[Sistema de Numeração Decimal - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Diferenciar **algarismo** de **número** e **valor absoluto** de **valor relativo**.
- Ler e escrever números grandes usando **ordens e classes**.
- **Decompor** um número em potências de 10.
- Entender que a base 10 é uma escolha e converter números entre a **base 2 (binário)** e a base 10.

---

## 1. Intuição: agrupar de 10 em 10

Imagine contar 347 palitos. Contar um por um é cansativo, então você faz montinhos:
- a cada **10 palitos**, amarra um feixe (uma **dezena**);
- a cada **10 feixes**, amarra um pacote (uma **centena**).

No fim, sobram **3 pacotes, 4 feixes e 7 palitos soltos**. Escrevemos **347**: a posição diz *de que tipo* é cada quantidade.

> [!tip] A ideia central
> O "3" de 347 não vale 3: vale **3 centenas = 300**. O mesmo símbolo vale coisas diferentes conforme a casa em que está. Isso é um **sistema posicional**.

E o **zero**? Ele marca uma casa vazia. Em **305**, há 3 centenas, **nenhuma** dezena e 5 unidades. Sem o zero, não daria para distinguir 305 de 35.

## 2. Algarismo × número

- **Algarismos** são os 10 símbolos: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9.
- **Números** são as quantidades que escrevemos combinando algarismos.

Assim como as letras formam palavras, os algarismos formam números. O número 2026 tem 4 algarismos.

## 3. Ordens e classes

Cada posição é uma **ordem**. A cada três ordens, temos uma **classe**:

| Classe | Bilhões | | | Milhões | | | Milhares | | | Unidades simples | | |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Ordem | C | D | U | C | D | U | C | D | U | C | D | U |
| Exemplo | | | 3 | 0 | 4 | 5 | 2 | 0 | 0 | 0 | 1 | 7 |

O número acima é **3.045.200.017**: *três bilhões, quarenta e cinco milhões, duzentos mil e dezessete*.

> [!example] Como ler um número grande
> 1. Separe em grupos de 3 algarismos, **da direita para a esquerda**: `3 | 045 | 200 | 017`.
> 2. Leia cada grupo como um número de até 3 algarismos e diga o nome da classe: "três **bilhões**", "quarenta e cinco **milhões**", "duzentos **mil**", "dezessete".

No Brasil, o **ponto** separa as classes (1.000) e a **vírgula** separa os decimais (2,5). Em vários outros países e no código, é o contrário.

## 4. Valor absoluto e valor relativo

- **Valor absoluto**: o valor do algarismo sozinho. No 5.372, o 3 tem valor absoluto **3**.
- **Valor relativo** (ou posicional): o valor pela posição. No 5.372, o 3 está nas centenas, então vale **300**.

## 5. Decomposição

Todo número é uma soma de "algarismo × valor da casa":

$$
5372 = 5 \cdot 1000 + 3 \cdot 100 + 7 \cdot 10 + 2 \cdot 1
$$

E como $1000 = 10^3$, $100 = 10^2$, $10 = 10^1$ e $1 = 10^0$:

$$
5372 = 5 \cdot 10^3 + 3 \cdot 10^2 + 7 \cdot 10^1 + 2 \cdot 10^0
$$

Por isso o sistema se chama **decimal**, ou **de base 10**. Você vai entender bem as potências em [[Potenciação]]; por enquanto, $10^3$ significa $10 \cdot 10 \cdot 10$.

> [!tip] Um truque que vai aparecer muito
> Um número de dois algarismos com dezena $a$ e unidade $b$ vale $10a + b$. Por exemplo, $47 = 10 \cdot 4 + 7$. Essa forma resolve muitos problemas de olimpíada.

## 6. Bônus: outras bases (o binário)

Usamos base 10 provavelmente porque temos 10 dedos. Mas a ideia funciona com **qualquer** tamanho de grupo. O computador usa **base 2**: só existem os algarismos 0 e 1, e cada casa vale **2 vezes** a da direita.

| Casa | $2^4 = 16$ | $2^3 = 8$ | $2^2 = 4$ | $2^1 = 2$ | $2^0 = 1$ |
|---|---|---|---|---|---|
| $10110_2$ | 1 | 0 | 1 | 1 | 0 |

$$
10110_2 = 16 + 4 + 2 = 22
$$

**De decimal para binário**, divida sucessivamente por 2 e leia os restos **de baixo para cima**:

| Divisão | Quociente | Resto |
|---|---|---|
| 22 ÷ 2 | 11 | **0** |
| 11 ÷ 2 | 5 | **1** |
| 5 ÷ 2 | 2 | **1** |
| 2 ÷ 2 | 1 | **0** |
| 1 ÷ 2 | 0 | **1** |

Lendo de baixo para cima: $10110_2$. ✔️

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: valor relativo
> No número **84.619**, qual é o valor relativo do 4?
> O 4 está na **unidade de milhar** (4ª casa da direita para a esquerda), então vale $4 \cdot 1000 = 4000$.

> [!example] Exemplo 2: escrever com algarismos
> "Dois milhões, cinquenta mil e dezessete."
> Monte as classes: milhões = **2**, milhares = **050**, unidades = **017**. Resultado: **2.050.017**.
> Repare nos zeros: cada classe, menos a primeira, precisa ter **3 algarismos**.

> [!example] Exemplo 3: decompor
> $40608 = 4 \cdot 10^4 + 0 \cdot 10^3 + 6 \cdot 10^2 + 0 \cdot 10^1 + 8 \cdot 10^0 = 40000 + 600 + 8$

> [!example] Exemplo 4: contar números
> Quantos números de 3 algarismos existem?
> Vão de 100 até 999. Quantidade $= 999 - 100 + 1 = 900$.
> (O "+1" existe porque contamos os dois extremos. É como contar os dias de 10 a 12: são 3 dias, não 2.)

> [!example] Exemplo 5: binário
> Converta 13 para binário: $13 = 8 + 4 + 1 = 1 \cdot 8 + 1 \cdot 4 + 0 \cdot 2 + 1 \cdot 1 \Rightarrow 1101_2$

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| "Dois mil e cinco" = 205 ou 20005 | **2005** | A classe dos milhares tem o 2; a classe das unidades precisa de 3 algarismos: **005** |
| "O número 7 de 4.712 vale 7" | Vale **700** | O valor relativo depende da posição |
| Contar de 100 a 999 como $999 - 100 = 899$ | $999 - 100 + 1 = 900$ | Os dois extremos entram na contagem |
| Confundir "algarismo" com "número" | 352 é um **número** de 3 **algarismos** | |

---

## 💻 Conexão com programação e ML

- **Extrair algarismos** é um padrão clássico: `n % 10` dá o último algarismo e `n / 10` (divisão inteira) remove o último algarismo. Isso é a decomposição posicional em código.
- `Convert.ToString(22, 2)` retorna `"10110"`, e `Convert.ToInt32("10110", 2)` retorna `22`. Hexadecimal (base 16) é o mesmo raciocínio: a cor `#FF0000` é $FF_{16} = 255$ de vermelho.
- **Cultura importa:** em pt-BR, `double.Parse("1.000")` dá **1000**; com `CultureInfo.InvariantCulture`, dá **1**. É a diferença ponto/vírgula da seção 3.
- **Em ML:** os pesos de um modelo são guardados em binário (`float32`, `float16`). "Quantizar" um modelo para `int8` é representar os números com menos casas binárias, trocando precisão por memória.

---

## 🔗 Conexões
- **Usa:** só a ideia de contar.
- **É usado em:**
  - [[Operações Fundamentais]]: os algoritmos de "vai um" e "empresta" são reagrupamentos de casas.
  - [[Múltiplos, Divisores e Primos]]: os critérios de divisibilidade por 2, 5 e 10 funcionam *por causa* do valor posicional.
  - [[Números Decimais]]: as casas continuam à direita da vírgula (décimos, centésimos…).
  - [[Potenciação]]: a decomposição usa potências de 10, e a [[Potenciação#6. Notação científica|notação científica]] nasce daqui.
- **Mais adiante:** [[Progressão Geométrica]] (as casas 1, 10, 100… formam uma PG) e [[Função Exponencial]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Qual é a diferença entre valor absoluto e valor relativo? Dê um exemplo.
2. Por que o zero é indispensável num sistema posicional?
3. Quantas ordens tem uma classe? Quais são as classes até os bilhões?
4. Escreva $7.030.402$ decomposto em potências de 10.
5. Um número tem dezena $a$ e unidade $b$. Como escrevê-lo em função de $a$ e $b$?
6. Quanto vale $111_2$ em decimal? E como se converte 6 para binário?
