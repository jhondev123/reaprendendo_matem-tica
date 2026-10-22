---
tipo: conceito
tema: Álgebra
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Inequações
  - Desigualdades
  - Intervalos reais
tags:
  - algebra
---
# Inequações do 1º Grau

> [!abstract] Em uma frase
> Uma inequação se resolve **como uma equação**, com uma única diferença: ao **multiplicar ou dividir por um número negativo**, o sinal da desigualdade **inverte**. A resposta não é um número, mas um **intervalo** da reta.

**Tema:** [[Álgebra]] · **Pré-requisitos:** [[Equações do 1º Grau]], [[Conjuntos Numéricos]] · **Próximo:** [[Sistemas de Equações]]
**Praticar:** [[Inequações do 1º Grau - Exercícios]] · [[Inequações do 1º Grau - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Resolver inequações do 1º grau, **invertendo o sinal** quando necessário.
- Escrever a solução com a **notação de intervalos** e na reta.
- Resolver inequações duplas ($a < \dots < b$) e sistemas de inequações.
- Usar inequações em problemas de "a partir de quando compensa".

---

## 1. Os símbolos

| Símbolo | Lê-se | Exemplo verdadeiro |
|---|---|---|
| $<$ | menor que | $2 < 5$ |
| $>$ | maior que | $-1 > -3$ |
| $\leq$ | menor **ou igual** a | $4 \leq 4$ |
| $\geq$ | maior **ou igual** a | $7 \geq 2$ |

Uma inequação como $x + 3 > 7$ não tem uma solução só: **todo** número maior que 4 serve. A resposta é um **conjunto**.

## 2. Resolvendo: igual à equação…

Você pode somar ou subtrair o mesmo número dos dois lados, e multiplicar ou dividir por um número **positivo**, sem mexer no sinal:

$$3x - 2 < x + 6 \;\Rightarrow\; 2x < 8 \;\Rightarrow\; x < 4$$

## 3. …com UMA diferença

> [!danger] Multiplicou ou dividiu por negativo? Inverta o sinal!
> $$-3x > 12 \;\Rightarrow\; x < \frac{12}{-3} \;\Rightarrow\; x < -4$$

> [!question]- Por que inverte? (clique para abrir)
> Pegue uma desigualdade verdadeira: $2 < 5$. Multiplique os dois lados por $-1$: $-2$ e $-5$. Agora, $-2 > -5$ (na reta, $-2$ está à direita).
> Multiplicar por $-1$ é **espelhar a reta** em torno do zero: quem estava à direita passa para a esquerda. Por isso a ordem se inverte. (Lembre de [[Números Inteiros#1. A reta numérica|a reta numérica]].)

> [!tip] Um jeito de nunca errar
> Em vez de dividir por um negativo, **passe o termo com $x$ para o lado em que ele fica positivo**:
> $5 - x \geq 2 \;\Rightarrow\; 5 - 2 \geq x \;\Rightarrow\; x \leq 3$.

## 4. Intervalos: escrevendo a resposta

| Desigualdade | Intervalo | Na reta |
|---|---|---|
| $x > 2$ | $]2, +\infty[$ | bolinha **aberta** em 2, seta para a direita |
| $x \geq 2$ | $[2, +\infty[$ | bolinha **fechada** em 2 |
| $-1 \leq x < 3$ | $[-1, 3[$ | fechada em −1, aberta em 3 |
| $x \leq 0$ | $]-\infty, 0]$ | fechada em 0, seta para a esquerda |

- **Colchete virado para dentro** $[\;]$: inclui o extremo (bolinha cheia ●).
- **Colchete virado para fora** $]\;[$: não inclui o extremo (bolinha vazia ○). Muitos livros usam parênteses: $(2, +\infty)$.
- O infinito **nunca** é incluído: sempre $]$ ou $[$ do lado dele.

```
x > 2:          ───────────○━━━━━━━━━━━━→
                          2
−1 ≤ x < 3:     ──────●━━━━━━━━━━━○──────
                     −1           3
```

Também se escreve como conjunto: $S = \{x \in \mathbb{R} \mid x > 2\}$ (lê-se "os reais $x$ tais que $x > 2$").

## 5. Inequações duplas

$-1 < 2x + 3 \leq 7$: faça a mesma operação **nas três partes**.
$$-1 - 3 < 2x \leq 7 - 3 \;\Rightarrow\; -4 < 2x \leq 4 \;\Rightarrow\; -2 < x \leq 2 \;\Rightarrow\; S = \,]-2, 2]$$

## 6. Sistemas de inequações

Resolva cada uma e faça a **interseção** (o que vale para todas ao mesmo tempo, o $\cap$ de [[Conjuntos Numéricos]]):
$$\begin{cases} 2x - 1 > 3 \\ x + 4 \leq 10 \end{cases} \Rightarrow \begin{cases} x > 2 \\ x \leq 6 \end{cases} \Rightarrow S = \,]2, 6]$$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: com frações
> $\frac{x}{2} - 1 > \frac{x}{3}$. Multiplicando por 6 (que é **positivo**, então o sinal não muda): $3x - 6 > 2x \Rightarrow x > 6$.

> [!example] Exemplo 2: com decimais e sinal invertido
> $0{,}2x - 1{,}5 \geq 0{,}5x + 0{,}3$. Multiplicando por 10: $2x - 15 \geq 5x + 3 \Rightarrow -3x \geq 18 \Rightarrow x \leq -6$ (dividiu por $-3$: inverteu).

> [!example] Exemplo 3: coeficiente irracional negativo
> $(1 - \sqrt{2})\,x > 1 - \sqrt{2}$. Como $\sqrt{2} \approx 1{,}41$, o coeficiente $1 - \sqrt{2}$ é **negativo**. Dividindo por ele, o sinal inverte: $x < 1$.
> ⚠️ Antes de dividir, sempre se pergunte: **esse número é positivo ou negativo?**

> [!example] Exemplo 4: quando compensa?
> Plano A: R\$ 50 fixos + R\$ 0,10 por minuto. Plano B: R\$ 30 fixos + R\$ 0,20 por minuto. A partir de quantos minutos o plano A é mais barato?
> $50 + 0{,}1m < 30 + 0{,}2m \Rightarrow 20 < 0{,}1m \Rightarrow m > 200$. **Acima de 200 minutos.**

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $-2x > 6 \Rightarrow x > -3$ | $x < -3$ | dividiu por negativo: inverta |
| $2x > -6 \Rightarrow x < -3$ | $x > -3$ | dividiu por **positivo**; o sinal do **resultado** não importa |
| $x \geq 2$ como $]2, +\infty[$ | $[2, +\infty[$ | "ou igual" significa extremo fechado |
| $[3, +\infty]$ | $[3, +\infty[$ | o infinito nunca é incluído |
| Sistema: unir as soluções | **interseção** | as duas condições valem **ao mesmo tempo** |

---

## 💻 Conexão com programação e ML

- Todo `if (x >= limite)` é uma inequação. **Classificar** é decidir de que lado de uma desigualdade um ponto está.
- O **perceptron**, o neurônio artificial mais simples, classifica como positivo quando $w \cdot x + b \geq 0$. Resolver essa inequação dá a **fronteira de decisão** do modelo: com $w = 2$ e $b = -3$, é positivo quando $x \geq 1{,}5$.
- **Limiar de decisão:** um classificador retorna uma probabilidade $p$ e decide "sim" se $p \geq 0{,}5$. Mudar o limiar troca precisão por *recall*.
- **Clipping:** `Math.Clamp(v, -1, 1)` força $-1 \leq v \leq 1$. O *gradient clipping* faz isso para impedir que o treino "exploda".

---

## 🔗 Conexões
- **Usa:** [[Equações do 1º Grau]] (o mesmo método), [[Números Inteiros]] (por que o sinal inverte), [[Conjuntos Numéricos]] (a reta real e a interseção).
- **É usado em:** [[Sistemas de Equações]] (que também tratam de várias condições juntas).
- **Mais adiante:**
  - [[Função Afim]]: "onde a reta está acima do eixo?" é uma inequação.
  - [[Função Quadrática]]: as inequações do 2º grau.
  - [[Função Modular]]: $\lvert x \rvert < 3 \iff -3 < x < 3$.
  - [[Conceito de Função]]: o domínio costuma ser um intervalo.

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Qual é a única diferença entre resolver uma equação e uma inequação?
2. Mostre, com $3 < 7$, por que multiplicar por $-2$ inverte o sinal.
3. Escreva $-5 < x \leq 1$ como intervalo e desenhe na reta.
4. Resolva $4 - 3x \leq 10$ sem dividir por negativo.
5. Por que o infinito nunca fica com colchete fechado?
6. Num sistema de inequações, faz-se a união ou a interseção? Por quê?
