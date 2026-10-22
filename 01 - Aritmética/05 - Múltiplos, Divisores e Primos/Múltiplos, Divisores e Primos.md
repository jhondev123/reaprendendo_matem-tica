---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Divisibilidade
  - Números primos
  - Fatoração em primos
  - Critérios de divisibilidade
tags:
  - aritmetica
---
# Múltiplos, Divisores e Primos

> [!abstract] Em uma frase
> Os **primos** são os "átomos" dos números naturais: todo número maior que 1 se escreve **de um único jeito** como produto de primos, e isso revela todos os seus divisores.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Operações Fundamentais]] · **Próximo:** [[MMC e MDC]]
**Praticar:** [[Múltiplos, Divisores e Primos - Exercícios]] · [[Múltiplos, Divisores e Primos - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Listar múltiplos e divisores, achando os divisores **aos pares**.
- Usar os **critérios de divisibilidade** por 2, 3, 4, 5, 6, 9 e 10.
- Reconhecer **números primos** e testar se um número é primo.
- **Fatorar** um número em primos e contar quantos divisores ele tem.

---

## 1. Múltiplo e divisor: a mesma relação, vista dos dois lados

$$12 = 3 \cdot 4$$

- 12 é **múltiplo** de 3 (e de 4).
- 3 é **divisor** de 12, ou seja, 3 **divide** 12. Escreve-se $3 \mid 12$.

Em geral, $a$ é múltiplo de $b$ quando $a = b \cdot k$ para algum natural $k$, isto é, quando a [[Operações Fundamentais#6. Divisão com resto|divisão]] $a \div b$ tem **resto zero**.

| | Múltiplos de 6 | Divisores de 12 |
|---|---|---|
| Lista | $0, 6, 12, 18, 24, \dots$ | $1, 2, 3, 4, 6, 12$ |
| Quantidade | **infinitos** | **finitos** |

> [!tip] Ache os divisores aos pares
> Para $36$: $\;1 \cdot 36,\; 2 \cdot 18,\; 3 \cdot 12,\; 4 \cdot 9,\; 6 \cdot 6$. Ao chegar em $6 \cdot 6$ (ou seja, em $\sqrt{36}$), pode parar: os pares começariam a se repetir.
> Divisores de 36: $1, 2, 3, 4, 6, 9, 12, 18, 36$.

## 2. Critérios de divisibilidade

| Por | Regra | Exemplo |
|---|---|---|
| **2** | termina em algarismo par | 3.47**8** ✔️ |
| **3** | a soma dos algarismos é múltipla de 3 | 2.346 → $2+3+4+6 = 15$ ✔️ |
| **4** | os dois últimos algarismos formam múltiplo de 4 | 1.3**24** → 24 ✔️ |
| **5** | termina em 0 ou 5 | 1.23**5** ✔️ |
| **6** | é divisível por 2 **e** por 3 | 2.346 ✔️ |
| **9** | a soma dos algarismos é múltipla de 9 | 7.281 → $18$ ✔️ |
| **10** | termina em 0 | 4.5**0** ✔️ |

> [!question]- Por que o critério do 3 e do 9 funciona? (clique para abrir)
> Pelo [[Sistema de Numeração Decimal|valor posicional]], $2346 = 2 \cdot 1000 + 3 \cdot 100 + 4 \cdot 10 + 6$.
> Como $10 = 9 + 1$, $100 = 99 + 1$ e $1000 = 999 + 1$:
> $$2346 = \underbrace{2 \cdot 999 + 3 \cdot 99 + 4 \cdot 9}_{\text{múltiplo de 9 (e de 3)}} + \underbrace{(2 + 3 + 4 + 6)}_{\text{soma dos algarismos}}$$
> A primeira parte é sempre divisível por 9 (e por 3). Então o número inteiro é divisível por 3 ou por 9 **exatamente quando** a soma dos algarismos é.

## 3. Números primos

Um número é **primo** quando tem **exatamente dois divisores**: 1 e ele mesmo.

$$2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, \dots$$

- O **1 não é primo** (tem só um divisor).
- O **2 é o único primo par**.
- Números maiores que 1 que não são primos são **compostos**: $12 = 2 \cdot 6$.

**Como testar se $n$ é primo:** tente dividir por **2, 3, 5, 7, 11, …** apenas até $\sqrt{n}$. Se nenhum desses primos dividir $n$, ele é primo.
*Exemplo:* $97$. Como $\sqrt{97} \approx 9{,}8$, basta testar 2, 3, 5 e 7. Nenhum divide 97, então **97 é primo**.

> [!info] Curiosidade: os primos nunca acabam
> Euclides provou, há uns 2.300 anos, que existem infinitos primos. Suponha uma lista "completa" de primos e multiplique todos eles; some 1 ao resultado. O novo número deixa resto 1 na divisão por cada primo da lista, então ou ele é primo, ou tem um fator primo que não estava na lista. Em qualquer caso, a lista não estava completa.

## 4. Fatoração em primos

> [!important] Teorema Fundamental da Aritmética
> Todo número natural maior que 1 é primo ou se escreve como **produto de primos**, de um **único** jeito (a menos da ordem dos fatores).

Método das divisões sucessivas, sempre pelo **menor primo possível**:

| | |
|---|---|
| 360 | 2 |
| 180 | 2 |
| 90 | 2 |
| 45 | 3 |
| 15 | 3 |
| 5 | 5 |
| 1 | |

$$360 = 2 \cdot 2 \cdot 2 \cdot 3 \cdot 3 \cdot 5 = 2^3 \cdot 3^2 \cdot 5$$

(Os expoentes são [[Potenciação|potências]]: $2^3 = 2 \cdot 2 \cdot 2$.)

## 5. Contando divisores

Um divisor de $360 = 2^3 \cdot 3^2 \cdot 5^1$ é formado escolhendo **quantos** 2, quantos 3 e quantos 5 entram nele:
- do 2: 0, 1, 2 ou 3 → **4** opções
- do 3: 0, 1 ou 2 → **3** opções
- do 5: 0 ou 1 → **2** opções

$$\text{nº de divisores} = (3+1)(2+1)(1+1) = 4 \cdot 3 \cdot 2 = 24$$

**Regra:** some 1 a cada expoente e multiplique. (É o [[Princípio Fundamental da Contagem]], que você vai ver mais adiante.)

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1
> Divisores de 50, aos pares: $1 \cdot 50$, $2 \cdot 25$, $5 \cdot 10$. Então são $1, 2, 5, 10, 25, 50$.

> [!example] Exemplo 2
> 7.452 é divisível por 6? Termina em 2, então é par ✔️. A soma é $7 + 4 + 5 + 2 = 18$, múltipla de 3 ✔️. **Sim.** E por 9? A soma 18 também é múltipla de 9: **sim**.

> [!example] Exemplo 3
> 91 é primo? Como $\sqrt{91} \approx 9{,}5$, teste 2, 3, 5 e 7: $91 = 7 \cdot 13$. **Não é primo.** (O 91 engana muita gente!)

> [!example] Exemplo 4
> Fatore 84 e conte os divisores. $84 = 2^2 \cdot 3 \cdot 7$, então são $(2+1)(1+1)(1+1) = 12$ divisores.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| "1 é primo" | 1 **não** é primo | tem só um divisor |
| "51 é primo" | $51 = 3 \cdot 17$ | soma dos algarismos 6 → divisível por 3 |
| "Divisível por 2 e por 4 ⇒ divisível por 8" | falso: 12 | o critério do 6 funciona porque 2 e 3 são primos entre si; 2 e 4 não são |
| Fatorar $360 = 4 \cdot 90$ e parar | $2^3 \cdot 3^2 \cdot 5$ | a fatoração só termina quando **todos** os fatores são primos |
| Confundir múltiplo com divisor | 3 é divisor de 12; 12 é múltiplo de 3 | |

---

## 💻 Conexão com programação e ML

- **Testar primalidade** é um laço até $\sqrt{n}$: `for (int i = 2; i * i <= n; i++) if (n % i == 0) return false;`. Testar só até a raiz deixa o algoritmo muito mais rápido.
- **Criptografia RSA**, que protege o HTTPS, se baseia em multiplicar dois primos enormes ser fácil, mas fatorar o resultado ser praticamente impossível.
- **Hashing:** tabelas hash costumam usar tamanhos primos para espalhar melhor as chaves (o `Dictionary` do .NET faz isso internamente).
- **Em ML:** a fatoração é uma ideia que volta com outra roupa. *Fatorar matrizes* (como na SVD) é decompor um objeto complicado em peças simples, da mesma forma que $360 = 2^3 \cdot 3^2 \cdot 5$.

---

## 🔗 Conexões
- **Usa:** [[Operações Fundamentais]] (divisão com resto), [[Sistema de Numeração Decimal]] (por que os critérios funcionam).
- **É usado em:**
  - [[MMC e MDC]]: calculados direto da fatoração.
  - [[Frações e Equivalência]]: simplificar é dividir pelos fatores comuns.
  - [[Radiciação]]: $\sqrt{72} = \sqrt{2^3 \cdot 3^2} = 6\sqrt{2}$.
- **Na álgebra:** a [[Fatoração]] de polinômios é a mesma ideia, aplicada a expressões.
- **Mais adiante:** [[Princípio Fundamental da Contagem]] (contar divisores) e [[Autovalores e Autovetores]] (decompor matrizes).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Qual é a diferença entre "múltiplo de 5" e "divisor de 5"? Quantos existem de cada?
2. Enuncie os critérios de divisibilidade por 3, 4 e 9.
3. Por que o 1 não é primo? Por que basta testar divisores até $\sqrt{n}$?
4. O que diz o Teorema Fundamental da Aritmética?
5. Fatore 120 e diga quantos divisores ele tem.
6. Por que "divisível por 2 e por 3" garante "divisível por 6", mas "divisível por 2 e por 4" não garante "divisível por 8"?
