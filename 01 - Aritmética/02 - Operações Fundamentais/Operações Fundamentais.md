---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Quatro operações
  - Propriedade distributiva
  - Divisão com resto
tags:
  - aritmetica
---
# Operações Fundamentais

> [!abstract] Em uma frase
> As quatro operações têm **propriedades** que deixam você reorganizar as contas para facilitá-las. A subtração e a divisão são as **operações inversas** da adição e da multiplicação.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Sistema de Numeração Decimal]] · **Próximo:** [[Números Inteiros]]
**Praticar:** [[Operações Fundamentais - Exercícios]] · [[Operações Fundamentais - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Nomear os termos de cada operação.
- Usar as propriedades **comutativa, associativa e distributiva** para fazer contas de cabeça.
- Escrever e usar a **relação fundamental da divisão**: $D = d \cdot q + r$.
- Explicar **por que não existe divisão por zero**.
- Conferir uma conta usando a operação inversa.

---

## 1. Intuição: o que cada operação faz

| Operação | Ideia | Exemplo |
|---|---|---|
| **Adição** | juntar | 3 maçãs + 4 maçãs = 7 maçãs |
| **Subtração** | tirar, ou saber "quanto falta" e "qual a diferença" | tenho 10 reais e gasto 3: sobram 7 |
| **Multiplicação** | somar parcelas iguais repetidas vezes, ou calcular a área de um retângulo | $4 \cdot 3 = 3 + 3 + 3 + 3 = 12$ |
| **Divisão** | repartir em partes iguais, ou ver "quantas vezes cabe" | 12 balas para 4 pessoas: 3 para cada |

> [!tip] Multiplicação como área
> $4 \cdot 3$ é um retângulo de 4 linhas por 3 colunas: 12 quadradinhos. Girando o retângulo, ele vira $3 \cdot 4$ e a área não muda. Esse é o motivo da propriedade comutativa.

## 2. Os nomes dos termos

| Operação | Termos |
|---|---|
| $8 + 5 = 13$ | 8 e 5 são **parcelas**; 13 é a **soma** |
| $13 - 5 = 8$ | 13 é o **minuendo**; 5 é o **subtraendo**; 8 é a **diferença** (ou resto) |
| $4 \cdot 6 = 24$ | 4 e 6 são **fatores**; 24 é o **produto** |
| $24 \div 6 = 4$ | 24 é o **dividendo**; 6 é o **divisor**; 4 é o **quociente** |

## 3. Propriedades

Valem para a **adição** e para a **multiplicação**:

| Propriedade | Adição | Multiplicação | Em palavras |
|---|---|---|---|
| **Comutativa** | $a + b = b + a$ | $a \cdot b = b \cdot a$ | a ordem não altera o resultado |
| **Associativa** | $(a + b) + c = a + (b + c)$ | $(a \cdot b) \cdot c = a \cdot (b \cdot c)$ | o agrupamento não altera o resultado |
| **Elemento neutro** | $a + 0 = a$ | $a \cdot 1 = a$ | somar 0 e multiplicar por 1 não mudam nada |
| **Elemento absorvente** | n/a | $a \cdot 0 = 0$ | qualquer coisa vezes zero dá zero |

E a mais importante de todas, que liga as duas operações:

$$
\textbf{Distributiva:} \quad a \cdot (b + c) = a \cdot b + a \cdot c
$$

> [!example] A distributiva como área
> Um retângulo de altura 3 e largura $(4 + 2)$ tem área $3 \cdot 6 = 18$. Cortando-o em dois retângulos, um de largura 4 e outro de largura 2, a área é $3 \cdot 4 + 3 \cdot 2 = 12 + 6 = 18$. É o mesmo retângulo.

> [!warning] A subtração e a divisão **não** são comutativas nem associativas
> - $10 - 3 = 7$, mas $3 - 10 \neq 7$.
> - $(12 \div 6) \div 2 = 1$, mas $12 \div (6 \div 2) = 4$.

## 4. Cálculo mental com as propriedades

As propriedades são **ferramentas** para simplificar contas:

- **Agrupe para fechar dezenas** (associativa e comutativa): $38 + 47 + 62 = (38 + 62) + 47 = 100 + 47 = 147$
- **Procure os pares 4·25, 2·5, 8·125** (que dão 100, 10 e 1000): $4 \cdot 17 \cdot 25 = (4 \cdot 25) \cdot 17 = 1700$
- **Quebre números perto de dezenas redondas** (distributiva): $7 \cdot 98 = 7 \cdot (100 - 2) = 700 - 14 = 686$
- **Coloque o fator comum em evidência** (distributiva ao contrário): $13 \cdot 45 + 13 \cdot 55 = 13 \cdot (45 + 55) = 1300$

A última ideia, a de **"colocar em evidência"**, será a base da [[Fatoração]] na álgebra.

## 5. Operações inversas

- A subtração desfaz a adição: $a - b = c \iff c + b = a$
- A divisão desfaz a multiplicação: $a \div b = c \iff c \cdot b = a$

Use isso para **conferir** contas: se $1008 \div 24 = 42$, então $42 \cdot 24$ tem que dar $1008$.

## 6. Divisão com resto

Nem toda divisão é exata. Dividindo 47 balas entre 5 pessoas, cada uma recebe 9 e **sobram 2**:

$$
\underbrace{47}_{\text{dividendo}} = \underbrace{5}_{\text{divisor}} \cdot \underbrace{9}_{\text{quociente}} + \underbrace{2}_{\text{resto}}
$$

> [!important] Relação fundamental da divisão
> $$D = d \cdot q + r, \qquad \text{com } 0 \leq r < d$$
> O resto é **sempre menor que o divisor**. Se sobrasse 5 ou mais, daria para entregar mais uma bala para cada pessoa.

Essa relação aparece em muitos problemas: dias da semana (divisão por 7), horas (por 24 ou por 12), grupos, ônibus, lotes…

## 7. Por que não se divide por zero

Lembre que $a \div b = c$ significa $c \cdot b = a$.

- $6 \div 0 = ?$ Seria um número que, **multiplicado por 0, dá 6**. Não existe, pois tudo vezes zero dá zero.
- $0 \div 0 = ?$ Qualquer número serve ($5 \cdot 0 = 0$, $7 \cdot 0 = 0$…), então o resultado não fica determinado.
- Já $0 \div 6 = 0$ está **certo**, porque $0 \cdot 6 = 0$.

Conclusão: **a divisão por zero não está definida.**

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: associativa
> $25 + 68 + 75 = (25 + 75) + 68 = 100 + 68 = 168$

> [!example] Exemplo 2: distributiva
> $13 \cdot 99 = 13 \cdot (100 - 1) = 1300 - 13 = 1287$

> [!example] Exemplo 3: divisão com resto num problema
> Uma excursão tem 250 alunos e cada ônibus leva 40. Quantos ônibus são necessários?
> $250 = 40 \cdot 6 + 10$. Seis ônibus levam 240 alunos e **sobram 10**, que precisam de mais um ônibus. Resposta: **7 ônibus**.
> ⚠️ O quociente (6) não é a resposta: o contexto manda arredondar **para cima**.

> [!example] Exemplo 4: dias da semana
> Hoje é segunda-feira. Que dia será daqui a 100 dias?
> A cada 7 dias, o dia da semana se repete. $100 = 7 \cdot 14 + 2$: as 14 semanas completas voltam à segunda, e os **2 dias** que restam levam a **quarta-feira**.

> [!example] Exemplo 5: evidência
> $9 \cdot 48 + 48 = 9 \cdot 48 + 1 \cdot 48 = (9 + 1) \cdot 48 = 480$

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $9 \div 0 = 0$ | não existe | nenhum número vezes 0 dá 9 |
| $0 \div 9$ "não existe" | $0 \div 9 = 0$ | $0 \cdot 9 = 0$ |
| $47 \div 5 = 8$, resto 7 | $9$, resto 2 | o resto tem que ser menor que o divisor |
| $2 \cdot (3 \cdot 4) = (2 \cdot 3) \cdot (2 \cdot 4)$ | $2 \cdot (3 \cdot 4) = 24$ | a distributiva vale para **soma ou subtração** dentro dos parênteses, não para multiplicação |
| $20 - 5 - 3 = 20 - (5 - 3) = 18$ | $20 - 5 - 3 = 12$ | a subtração não é associativa |

---

## 💻 Conexão com programação e ML

- Em C#, com `int`, o operador `/` faz **divisão inteira** (`47 / 5 == 9`) e `%` dá o **resto** (`47 % 5 == 2`). É exatamente a relação $D = d \cdot q + r$: `47 == 5 * (47 / 5) + 47 % 5`.
- `7 / 0` com `int` lança `DivideByZeroException`. Com `double`, `7.0 / 0` dá `Infinity` e `0.0 / 0` dá `NaN` ("not a number"). O computador também reconhece que esses resultados não são números comuns.
- Arredondar uma divisão **para cima** sem usar `Math.Ceiling`: `(total + tamanho - 1) / tamanho`.
- **Em ML:** treinar com 1000 exemplos em *batches* de 64 dá $1000 = 64 \cdot 15 + 40$: são 15 lotes cheios e um último com 40, ou seja, **16 lotes por época**. Já a propriedade **distributiva** é o que torna as funções lineares tão "bem-comportadas": $w \cdot (x_1 + x_2) = w x_1 + w x_2$.

---

## 🔗 Conexões
- **Usa:** [[Sistema de Numeração Decimal]].
- **É usado em:**
  - [[Números Inteiros]]: as mesmas propriedades valem com números negativos.
  - [[Expressões Numéricas]]: a ordem das operações.
  - [[Múltiplos, Divisores e Primos]]: "divisão exata" é o que define um divisor.
  - [[Frações e Equivalência]]: uma fração é uma divisão.
- **Na álgebra:** a distributiva é a base de [[Monômios e Polinômios]] (multiplicar polinômios), de [[Produtos Notáveis]] e de [[Fatoração]] (colocar em evidência).
- **Mais adiante:** a soma de Gauss reaparece em [[Soma dos Termos de PA e PG]] e em [[Somatório e Produtório]]; o resto da divisão volta em problemas de ciclos e calendários.

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Quais propriedades valem para a adição e a multiplicação, mas não para a subtração e a divisão?
2. Enuncie a propriedade distributiva e desenhe um retângulo que a explique.
3. Calcule $8 \cdot 99$ de cabeça. Qual propriedade você usou? 8 x 100 - 8 = 792
4. Escreva a relação fundamental da divisão. Por que o resto precisa ser menor que o divisor? porque ele é o resto da distribuição, onde não foi possível fazer a divisão completa.
5. Explique, usando a operação inversa, por que $5 \div 0$ não existe e por que $0 \div 5 = 0$. porque 5/0 =0 implicaria que existe um numero multiplicado por 0 que daria 5 e seria incorreto, agora 0/5 = 0 implica que existe um número que multiplicado por 5 daria 0, ou seja 0 e nesse caso existe
6. Como você confere se $391 \div 17 = 23$ sem refazer a divisão? Quociente x Divisor = Dividendo, logo 23x17=391
