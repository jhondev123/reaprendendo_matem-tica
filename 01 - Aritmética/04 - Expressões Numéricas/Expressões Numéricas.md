---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Ordem das operações
  - Precedência
tags:
  - aritmetica
---
# Expressões Numéricas

> [!abstract] Em uma frase
> Uma expressão tem **uma ordem de resolução** que todos seguem. Sem ela, a mesma conta daria resultados diferentes, como num código sem regras de precedência.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Operações Fundamentais]], [[Números Inteiros]] · **Próximo:** [[Múltiplos, Divisores e Primos]]
**Praticar:** [[Expressões Numéricas - Exercícios]] · [[Expressões Numéricas - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Resolver expressões com parênteses, colchetes e chaves, de dentro para fora.
- Aplicar a ordem: **potências e raízes → multiplicações e divisões → adições e subtrações**.
- Resolver multiplicações e divisões "do mesmo nível" **da esquerda para a direita**.
- Tratar o **traço de fração** como um parêntese.

---

## 1. A ordem (decore esta tabela)

| Prioridade | O quê | Observação |
|---|---|---|
| 1º | **Agrupamentos**: $(\;)$, depois $[\;]$, depois $\{\;\}$ | de dentro para fora |
| 2º | **Potências e raízes** | $2^3$, $\sqrt{9}$ |
| 3º | **Multiplicações e divisões** | na ordem em que aparecem, da esquerda para a direita |
| 4º | **Adições e subtrações** | na ordem em que aparecem, da esquerda para a direita |

> [!tip] Multiplicação e divisão estão no **mesmo** nível
> Não é "toda multiplicação antes de toda divisão". Resolva o que vier primeiro, da esquerda para a direita:
> $$8 \div 2 \cdot 4 = 4 \cdot 4 = 16 \qquad (\text{e não } 8 \div 8 = 1)$$
> O mesmo vale para soma e subtração: $10 - 3 + 2 = 9$ (e não $10 - 5 = 5$).

## 2. O traço de fração é um parêntese

$$\frac{6 + 4}{2} = \frac{10}{2} = 5 \qquad \text{e não} \qquad 6 + \frac{4}{2} = 8$$

Resolva o numerador e o denominador **inteiros** antes de dividir. Na hora de escrever em uma linha (ou no código), isso vira `(6 + 4) / 2`.

## 3. O sinal antes do parêntese

Um sinal de menos antes de um agrupamento **troca o sinal de tudo** o que está dentro (é a [[Operações Fundamentais|distributiva]] com $-1$):

$$-(3 - 5 + 2) = -3 + 5 - 2 = 0$$

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1
> $$\begin{aligned}
> &20 - 3 \cdot 4 + 2^3 \\
> &= 20 - 3 \cdot 4 + 8 && \text{(potência)} \\
> &= 20 - 12 + 8 && \text{(multiplicação)} \\
> &= 16 && \text{(da esquerda para a direita)}
> \end{aligned}$$

> [!example] Exemplo 2: agrupamentos
> $$\begin{aligned}
> &50 - \{\,3 \cdot [\,10 - (2 + 3)\,] + 4\,\} \\
> &= 50 - \{\,3 \cdot [\,10 - 5\,] + 4\,\} \\
> &= 50 - \{\,3 \cdot 5 + 4\,\} \\
> &= 50 - 19 = 31
> \end{aligned}$$

> [!example] Exemplo 3: com negativos e potência
> $$-2^2 + (-3)^2 \cdot 2 - 10 \div (-5) = -4 + 9 \cdot 2 + 2 = -4 + 18 + 2 = 16$$

> [!example] Exemplo 4: fração com expressão
> $$\frac{3^2 - 1}{2 \cdot (5 - 3)} = \frac{9 - 1}{2 \cdot 2} = \frac{8}{4} = 2$$

> [!example] Exemplo 5: com raiz
> $$\sqrt{16} + 2 \cdot \sqrt{25} - \sqrt{9 + 16} = 4 + 10 - \sqrt{25} = 14 - 5 = 9$$
> ⚠️ $\sqrt{9 + 16} = \sqrt{25} = 5$, e **não** $\sqrt{9} + \sqrt{16} = 7$. A raiz também age como um parêntese. (Mais em [[Radiciação]].)

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $2 + 3 \cdot 4 = 20$ | $14$ | a multiplicação vem antes da soma |
| $8 \div 2 \cdot 4 = 1$ | $16$ | mesmo nível: da esquerda para a direita |
| $10 - 3 + 2 = 5$ | $9$ | mesmo nível: da esquerda para a direita |
| $\frac{6+4}{2} = 6 + 2$ | $5$ | o traço de fração agrupa o numerador |
| $-(5 - 2) = -5 - 2$ | $-5 + 2 = -3$ | o menos troca o sinal de **todos** os termos |
| $\sqrt{9+16} = 3 + 4$ | $5$ | a raiz de uma soma não é a soma das raízes |

---

## 💻 Conexão com programação e ML

- O C# segue a mesma precedência: `2 + 3 * 4 == 14` e `8 / 2 * 4 == 16`.
- ⚠️ **O C# não tem operador de potência.** `2 ^ 3` é **XOR bit a bit** e vale `1`! Use `Math.Pow(2, 3)`.
- Ao passar uma fórmula para o código, todo traço de fração vira parênteses: $\frac{a + b}{c + d}$ → `(a + b) / (c + d)`. Esquecer esses parênteses é um bug clássico.
- **Em ML:** o erro quadrático médio $\frac{1}{n}\sum (y - \hat{y})^2$ segue exatamente esta ordem: primeiro a **diferença** (parênteses), depois o **quadrado** (potência), depois a **soma** e, por último, a **divisão** por $n$.

---

## 🔗 Conexões
- **Usa:** [[Operações Fundamentais]], [[Números Inteiros]].
- **É usado em:** praticamente tudo daqui em diante, com destaque para [[Operações com Frações]], [[Potenciação]] e [[Radiciação]].
- **Na álgebra:** calcular o **valor numérico** em [[Linguagem Algébrica]] é resolver uma expressão numérica; isolar $x$ em [[Equações do 1º Grau]] é "desfazer" a ordem das operações, de trás para a frente.
- **Treino:** as listas do [[Treino Misto de Aritmética]] são expressões que misturam todos os conjuntos.

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Qual é a ordem de prioridade das operações?
2. Em $12 \div 3 \cdot 2$, o que se faz primeiro? Quanto dá?
3. Por que $\frac{8 + 2}{2}$ não é $8 + 1$?
4. O que acontece com os sinais em $-(4 - 7 + 1)$?
5. Por que, em C#, `2 ^ 3` não dá 8?
6. Explique a ordem de cálculo de $\frac{1}{n}\sum (y - \hat{y})^2$.
