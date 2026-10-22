---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Polinômios
  - Monômios
  - Termos semelhantes
  - Multiplicação de polinômios
tags:
  - algebra
---
# Monômios e Polinômios

> [!abstract] Em uma frase
> Para **somar** polinômios, juntam-se só os **termos semelhantes** (mesmas letras com os mesmos expoentes), como "3 maçãs + 2 maçãs". Para **multiplicar**, usa-se a **distributiva**: cada termo de um multiplica cada termo do outro.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Linguagem Algébrica]], [[Potenciação]], [[Operações Fundamentais]] · **Próximo:** [[Produtos Notáveis]]
**Praticar:** [[Monômios e Polinômios - Exercícios]] · [[Monômios e Polinômios - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Fazer o bloco 🧮 de operações entre polinômios (soma, multiplicação e divisão)
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Reconhecer monômios, o seu grau e os termos semelhantes.
- **Somar e subtrair** polinômios sem errar os sinais.
- **Multiplicar** monômios e polinômios usando as propriedades das potências e a distributiva.
- Dividir um polinômio por um monômio e **por outro polinômio** (método da chave), achando o quociente e o resto.
- Calcular o valor de $P(x)$ e usar o **teorema do resto**.

---

## 1. Monômio

Um **monômio** é um número multiplicado por letras com expoentes naturais: $5x^2$, $\;-3ab$, $\;\frac{1}{2}y$, $\;7$.

- **Coeficiente:** o número, com o sinal ($-3$ em $-3ab$).
- **Parte literal:** as letras com os expoentes ($ab$).
- **Grau:** a soma dos expoentes das letras. $-4x^3y^2$ tem grau $3 + 2 = 5$; $\;7$ tem grau 0.

> [!warning] Não são monômios
> $\frac{1}{x}$ (seria $x^{-1}$) e $\sqrt{x}$ (seria $x^{1/2}$), porque os expoentes precisam ser naturais: 0, 1, 2…

## 2. Termos semelhantes: as "maçãs"

Dois monômios são **semelhantes** quando têm **a mesma parte literal**:

| Semelhantes ✅ | Não semelhantes ❌ |
|---|---|
| $3x$ e $-5x$ | $3x$ e $3y$ |
| $2x^2y$ e $7x^2y$ | $x^2$ e $x$ |
| $ab$ e $-4ba$ (a ordem não importa) | $x^2y$ e $xy^2$ |

Só termos semelhantes se juntam. Pense em $x$ como "maçã" e $y$ como "banana":
$$3x + 2x = 5x \quad (\text{3 maçãs} + \text{2 maçãs}) \qquad 3x + 2y \text{ fica assim} \quad (\text{não vira "5 maçananas"})$$

E $x^2$ e $x$ são frutas **diferentes** (uma é a área de um quadrado, a outra é o comprimento do lado): $x^2 + x$ não se simplifica.

## 3. Polinômio

Um **polinômio** é uma soma de monômios: $P(x) = 2x^3 - x^2 + 5x - 7$.
- A **forma reduzida** junta os semelhantes; a **ordenada** os coloca do maior para o menor expoente.
- O **grau** do polinômio é o maior grau entre os seus termos (aqui, 3).
- $P(2)$ é o [[Linguagem Algébrica#5. Valor numérico|valor numérico]] para $x = 2$: $\;2 \cdot 8 - 4 + 10 - 7 = 15$.

## 4. Adição e subtração

**Somar:** tire os parênteses e junte os semelhantes.
$$(3x^2 - 2x + 1) + (x^2 + 5x - 4) = (3 + 1)x^2 + (-2 + 5)x + (1 - 4) = 4x^2 + 3x - 3$$

**Subtrair:** o menos antes do parêntese **troca o sinal de todos os termos** de dentro.
$$(5a - 3b) - (2a - 4b) = 5a - 3b - 2a + 4b = 3a + b$$

> [!tip] Organize em colunas
> No caderno, escreva um polinômio embaixo do outro, alinhando os termos semelhantes, como na conta armada:
> ```
>   3x² − 2x + 1
> +  x² + 5x − 4
> ──────────────
>   4x² + 3x − 3
> ```

## 5. Multiplicação

**Monômio × monômio:** multiplique os coeficientes e **some os expoentes** das letras iguais ([[Potenciação#3. As propriedades (todas vêm da definição)|propriedade do produto]]):
$$(2x^3) \cdot (-3x^2) = -6x^5 \qquad (-a^2b) \cdot (4ab^3) = -4a^3b^4$$

**Monômio × polinômio:** distributiva.
$$3x(2x - 5) = 6x^2 - 15x$$

**Polinômio × polinômio:** **cada** termo do primeiro multiplica **cada** termo do segundo (o "chuveirinho"), e no fim junta-se o que for semelhante.
$$(x + 2)(x + 3) = x \cdot x + x \cdot 3 + 2 \cdot x + 2 \cdot 3 = x^2 + 3x + 2x + 6 = x^2 + 5x + 6$$

> [!example] O método da tabela (ótimo para não esquecer nenhum termo)
> $(2x - 1)(3x + 4)$:
>
> | $\times$ | $3x$ | $+4$ |
> |---|---|---|
> | $2x$ | $6x^2$ | $8x$ |
> | $-1$ | $-3x$ | $-4$ |
>
> Somando as quatro casas: $6x^2 + 8x - 3x - 4 = 6x^2 + 5x - 4$.
> A tabela é literalmente a **área** de um retângulo de lados $(2x - 1)$ e $(3x + 4)$, cortado em 4 pedaços.

> [!question]- Tente agora (clique para ver a resposta)
> Calcule $(x - 4)(x + 1)$.
> **Resposta:** $x^2 + x - 4x - 4 = x^2 - 3x - 4$

## 6. Divisão por monômio

Divida **cada termo** pelo monômio, subtraindo os expoentes:
$$\frac{12x^4 - 8x^3 + 4x^2}{4x^2} = 3x^2 - 2x + 1$$

## 7. Divisão de polinômio por polinômio (método da chave)

Funciona **exatamente** como a divisão armada de números, e vale a mesma [[Operações Fundamentais#6. Divisão com resto|relação fundamental]]:

$$P(x) = D(x) \cdot Q(x) + R(x), \qquad \text{com o grau de } R \text{ menor que o grau de } D$$

(dividendo = divisor × quociente + resto, como $47 = 5 \cdot 9 + 2$.)

**O ciclo, repetido até o resto ter grau menor que o divisor:**
1. **Divida** o primeiro termo do que sobrou pelo primeiro termo do divisor. Isso dá um termo do quociente.
2. **Multiplique** esse termo pelo divisor inteiro.
3. **Subtraia** do que sobrou (troque os sinais e some).

> [!example] Divisão exata: $(x^2 + 5x + 6) \div (x + 2)$
> ```
>   x² + 5x + 6   │ x + 2
> − x² − 2x       │───────
>   ─────────       x + 3
>        3x + 6
>      − 3x − 6
>      ────────
>             0
> ```
> 1. $x^2 \div x = x$. Multiplique: $x(x + 2) = x^2 + 2x$. Subtraia: sobra $3x + 6$.
> 2. $3x \div x = 3$. Multiplique: $3(x + 2) = 3x + 6$. Subtraia: sobra $0$.
>
> Quociente $x + 3$, resto $0$. Então $x^2 + 5x + 6 = (x + 2)(x + 3)$. Uma divisão exata é uma [[Fatoração]]!

> [!example] Divisão com resto: $(2x^3 - 3x^2 + 4x - 5) \div (x - 2)$
> 1. $2x^3 \div x = 2x^2$. $\;2x^2(x - 2) = 2x^3 - 4x^2$. Subtraindo: $-3x^2 + 4x^2 = x^2$, e sobra $x^2 + 4x - 5$.
> 2. $x^2 \div x = x$. $\;x(x - 2) = x^2 - 2x$. Subtraindo: sobra $6x - 5$.
> 3. $6x \div x = 6$. $\;6(x - 2) = 6x - 12$. Subtraindo: sobra $-5 + 12 = 7$.
>
> Quociente $Q(x) = 2x^2 + x + 6$, resto $R = 7$.
> **Verificação:** $(x - 2)(2x^2 + x + 6) + 7 = 2x^3 - 3x^2 + 4x - 12 + 7 = 2x^3 - 3x^2 + 4x - 5$ ✔️

> [!warning] Complete os termos que faltam com zero
> Para dividir $x^3 - 8$ por $x - 2$, escreva $x^3 + 0x^2 + 0x - 8$. Assim cada grau tem a sua "coluna" e nada se desalinha (é como o zero em 305, no [[Sistema de Numeração Decimal]]).

> [!tip] Teorema do resto
> O resto da divisão de $P(x)$ por $(x - a)$ é $P(a)$. No exemplo acima, $P(2) = 16 - 12 + 8 - 5 = 7$ ✔️. Em particular, se $P(a) = 0$, então $(x - a)$ **divide** $P(x)$, e $a$ é uma **raiz** do polinômio.

> [!info]- Atalho: dispositivo de Briot-Ruffini, para divisores da forma $(x - a)$ (clique para abrir)
> Para $(2x^3 - 3x^2 + 4x - 5) \div (x - 2)$, escreva só os coeficientes e o $a = 2$:
> ```
>  2 │  2   −3    4   −5
>    │       4    2   12
>    └───────────────────
>       2    1    6 │  7
> ```
> Desça o primeiro coeficiente (2). Depois, repita: multiplique por $a$ e some com o próximo: $2 \cdot 2 + (-3) = 1$; $\;1 \cdot 2 + 4 = 6$; $\;6 \cdot 2 + (-5) = 7$.
> A última linha dá o quociente $2x^2 + x + 6$ e o resto $7$. É o mesmo cálculo do método da chave, só que mais enxuto.

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: simplificar com sinais
> $$2(x - 3) - 3(2 - x) + x(x - 1) = 2x - 6 - 6 + 3x + x^2 - x = x^2 + 4x - 12$$

> [!example] Exemplo 2: com frações e decimais
> $$\left(\tfrac{1}{2}x - 0{,}5\right)(2x + 4) = x^2 + 2x - x - 2 = x^2 + x - 2$$

> [!example] Exemplo 3: três fatores
> $(x - 2)(x^2 + 2x + 4) = x^3 + 2x^2 + 4x - 2x^2 - 4x - 8 = x^3 - 8$. Quase tudo se cancela!

> [!example] Exemplo 4: geometria
> Um retângulo tem lados $2x + 3$ e $x - 1$.
> Área: $(2x + 3)(x - 1) = 2x^2 - 2x + 3x - 3 = 2x^2 + x - 3$.
> Perímetro: $2(2x + 3) + 2(x - 1) = 4x + 6 + 2x - 2 = 6x + 4$.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $3x + 2y = 5xy$ | não se simplifica | não são semelhantes |
| $x^2 + x^3 = x^5$ | não se simplifica | somar não é multiplicar; os expoentes só se somam na **multiplicação** |
| $2x \cdot 3x = 6x$ | $6x^2$ | $x \cdot x = x^2$ |
| $-(2x - 3) = -2x - 3$ | $-2x + 3$ | o menos troca **todos** os sinais |
| $(x + 2)(x + 3) = x^2 + 6$ | $x^2 + 5x + 6$ | faltaram os termos "cruzados" |
| $\frac{x^2 + 3}{x} = x + 3$ | $x + \frac{3}{x}$ | divida **cada** termo |

---

## 💻 Conexão com programação e ML

- Um polinômio pode ser guardado como um **array de coeficientes**: $2x^2 - 3x + 1$ vira `double[] p = { 1, -3, 2 }` (o índice é o expoente). Somar polinômios é somar os arrays posição a posição; multiplicar é uma **convolução**.
- **Método de Horner:** $2x^3 - x^2 + 5x - 7 = ((2x - 1)x + 5)x - 7$. Calcula o valor com só 3 multiplicações, num laço simples.
- **Em ML:**
  - A **regressão polinomial** ajusta $\hat{y} = w_0 + w_1x + w_2x^2 + \dots$. Polinômios de grau alto se "curvam demais" e decoram os dados (*overfitting*).
  - Cada neurônio calcula $w_1x_1 + w_2x_2 + \dots + b$, uma soma de termos (um polinômio de grau 1 em várias variáveis). A [[Somatório e Produtório|notação de somatório]] escreve isso de forma compacta.
  - Derivar polinômios é a primeira regra do cálculo ([[Regras de Derivação]]).

---

## 🔗 Conexões
- **Usa:** [[Linguagem Algébrica]], [[Potenciação]] (somar expoentes), [[Operações Fundamentais]] (a distributiva), [[Números Inteiros]] (sinais).
- **É usado em:**
  - [[Produtos Notáveis]]: multiplicações que aparecem tanto que merecem atalho.
  - [[Fatoração]]: o caminho inverso da multiplicação.
  - [[Frações Algébricas]] e [[Equações do 2º Grau]].
- **Mais adiante:** [[Função Quadrática]] (um polinômio de grau 2), [[Regras de Derivação]] e [[Integral Indefinida]] (derivar e integrar polinômios).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. O que são termos semelhantes? $x^2y$ e $xy^2$ são semelhantes?
2. Por que $3x + 2y$ não vira $5xy$? E por que $x^2 + x^3$ não vira $x^5$?
3. O que acontece com os sinais em $-(3x^2 - x + 4)$?
4. Como se multiplicam $(-2a^3b)$ e $(5ab^2)$?
5. Explique o "chuveirinho" e o método da tabela com $(x + 5)(x - 2)$.
6. Divida $9x^3 - 6x^2$ por $3x$.
7. Escreva a relação $P = D \cdot Q + R$ e explique o paralelo com $47 = 5 \cdot 9 + 2$.
8. Divida $x^2 - x - 6$ por $x - 3$ pelo método da chave. Como conferir sem refazer a divisão?
