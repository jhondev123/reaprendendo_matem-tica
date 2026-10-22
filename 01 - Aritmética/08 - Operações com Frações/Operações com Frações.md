---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Soma de frações
  - Divisão de frações
  - Inverso de uma fração
tags:
  - aritmetica
---
# Operações com Frações

> [!abstract] Em uma frase
> Para **somar**, as frações precisam ter o mesmo denominador (o mesmo "tamanho de pedaço"); para **multiplicar**, multiplica-se em linha reta; para **dividir**, multiplica-se pelo **inverso**.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Frações e Equivalência]], [[MMC e MDC]], [[Expressões Numéricas]] · **Próximo:** [[Números Decimais]]
**Praticar:** [[Operações com Frações - Exercícios]] · [[Operações com Frações - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Somar e subtrair frações com denominadores diferentes.
- Multiplicar frações **simplificando antes** (cancelamento cruzado).
- Dividir frações e explicar **por que** se inverte a segunda.
- Resolver expressões com frações, negativos e potências.

---

## 1. Adição e subtração

**Mesmo denominador:** some os numeradores e mantenha o denominador.
$$\frac{2}{7} + \frac{3}{7} = \frac{5}{7}$$
(2 pedaços de sétimo mais 3 pedaços de sétimo são 5 pedaços de sétimo.)

**Denominadores diferentes:** não dá para somar pedaços de tamanhos diferentes. Primeiro, reescreva as frações com o mesmo denominador, de preferência o [[MMC e MDC|MMC]].

$$\frac{1}{2} + \frac{1}{3} = \frac{3}{6} + \frac{2}{6} = \frac{5}{6}$$

> [!example] Passo a passo: $\frac{5}{6} - \frac{3}{4}$
> 1. $\text{mmc}(6, 4) = 12$
> 2. $\frac{5}{6} = \frac{10}{12}$ (multiplicou por 2) e $\frac{3}{4} = \frac{9}{12}$ (multiplicou por 3)
> 3. $\frac{10}{12} - \frac{9}{12} = \frac{1}{12}$

**Atalho** para duas frações (depois simplifique):
$$\frac{a}{b} + \frac{c}{d} = \frac{a \cdot d + b \cdot c}{b \cdot d}$$

**Inteiro com fração:** escreva o inteiro com o mesmo denominador. $3 - \frac{2}{5} = \frac{15}{5} - \frac{2}{5} = \frac{13}{5}$.

## 2. Multiplicação

Numerador vezes numerador, denominador vezes denominador:
$$\frac{a}{b} \cdot \frac{c}{d} = \frac{a \cdot c}{b \cdot d}$$

> [!tip] O "de" é uma multiplicação
> "$\frac{2}{3}$ de $\frac{3}{4}$ de uma pizza" $= \frac{2}{3} \cdot \frac{3}{4} = \frac{6}{12} = \frac{1}{2}$ pizza.
> Desenhe: um retângulo dividido em 4 colunas (pinte 3) e em 3 linhas (pinte 2 das 3 linhas da parte pintada). Sobram 6 quadradinhos de 12.

**Simplifique antes de multiplicar** (cancelamento cruzado): qualquer numerador pode ser simplificado com qualquer denominador, porque tudo é multiplicação.
$$\frac{2}{3} \cdot \frac{9}{14} = \frac{2 \cdot 9}{3 \cdot 14}$$
O 2 (em cima) simplifica com o 14 (embaixo), virando $\frac{1}{7}$, e o 9 (em cima) simplifica com o 3 (embaixo), virando $\frac{3}{1}$:
$$\frac{1 \cdot 3}{1 \cdot 7} = \frac{3}{7}$$
Assim os números ficam pequenos, e o resultado já sai irredutível.

**Inteiro vezes fração:** o inteiro multiplica **só o numerador**: $2 \cdot \frac{3}{4} = \frac{6}{4} = \frac{3}{2}$ (porque $2 = \frac{2}{1}$).

## 3. Inverso e divisão

O **inverso** de $\frac{a}{b}$ é $\frac{b}{a}$: o número que, multiplicado por ele, dá 1. O inverso de $\frac{3}{5}$ é $\frac{5}{3}$; o de $4$ é $\frac{1}{4}$; o de $-\frac{2}{7}$ é $-\frac{7}{2}$. **O zero não tem inverso.**

> [!important] Dividir é multiplicar pelo inverso
> $$\frac{a}{b} \div \frac{c}{d} = \frac{a}{b} \cdot \frac{d}{c}$$

> [!question]- Por que inverter? (clique para abrir)
> **Pela intuição:** $3 \div \frac{1}{4}$ pergunta "quantos quartos cabem em 3 inteiros?". Cada inteiro tem 4 quartos, então são $3 \cdot 4 = 12$. Dividir por $\frac{1}{4}$ é o mesmo que multiplicar por 4.
> **Pela álgebra:** uma divisão não muda se multiplicarmos o dividendo e o divisor pelo mesmo número. Multiplique os dois por $\frac{d}{c}$:
> $$\frac{a}{b} \div \frac{c}{d} = \left(\frac{a}{b} \cdot \frac{d}{c}\right) \div \underbrace{\left(\frac{c}{d} \cdot \frac{d}{c}\right)}_{=\,1} = \frac{a}{b} \cdot \frac{d}{c}$$

**Fração de frações** (o traço maior é uma divisão): "copia a de cima e multiplica pelo inverso da de baixo".
$$\frac{\;\frac{3}{4}\;}{\;\frac{9}{8}\;} = \frac{3}{4} \cdot \frac{8}{9} = \frac{24}{36} = \frac{2}{3}$$

## 4. Potência de fração

$$\left(\frac{a}{b}\right)^n = \frac{a^n}{b^n} \qquad \left(\frac{2}{3}\right)^2 = \frac{4}{9} \qquad \left(-\frac{1}{2}\right)^3 = -\frac{1}{8}$$

Sem parênteses, o expoente vale só para o numerador: $\frac{2^2}{3} = \frac{4}{3}$. Mais em [[Potenciação]].

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1: expressão
> $$\left(\frac{3}{4} - \frac{1}{2}\right) \cdot \left(\frac{2}{5} + \frac{1}{10}\right) = \frac{1}{4} \cdot \frac{5}{10} = \frac{1}{4} \cdot \frac{1}{2} = \frac{1}{8}$$

> [!example] Exemplo 2: com negativos
> $$-\frac{2}{3} + \left(-\frac{1}{2}\right) \cdot \left(-\frac{4}{3}\right) = -\frac{2}{3} + \frac{4}{6} = -\frac{2}{3} + \frac{2}{3} = 0$$

> [!example] Exemplo 3: fração de fração
> $$\frac{\frac{1}{2} + \frac{1}{3}}{\frac{1}{2} - \frac{1}{3}} = \frac{\frac{5}{6}}{\frac{1}{6}} = \frac{5}{6} \cdot \frac{6}{1} = 5$$

> [!example] Exemplo 4: problema de "fração do que sobrou"
> Gastei $\frac{1}{3}$ do salário com aluguel e $\frac{1}{4}$ **do restante** com mercado. Que fração do salário sobrou?
> Depois do aluguel, sobram $\frac{2}{3}$. O mercado leva $\frac{1}{4} \cdot \frac{2}{3} = \frac{1}{6}$ do salário. Sobram $\frac{2}{3} - \frac{1}{6} = \frac{4}{6} - \frac{1}{6} = \frac{3}{6} = \frac{1}{2}$.
> (Ou, mais rápido: sobram $\frac{3}{4}$ de $\frac{2}{3}$, ou seja, $\frac{3}{4} \cdot \frac{2}{3} = \frac{1}{2}$.)

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| $\frac{1}{2} + \frac{1}{3} = \frac{2}{5}$ | $\frac{5}{6}$ | **nunca** se somam os denominadores; antes, iguale-os |
| $2 \cdot \frac{3}{4} = \frac{6}{8}$ | $\frac{6}{4} = \frac{3}{2}$ | o inteiro multiplica só o numerador |
| $\frac{3}{4} \div \frac{9}{8} = \frac{4}{3} \cdot \frac{9}{8}$ | $\frac{3}{4} \cdot \frac{8}{9}$ | inverte-se a **segunda** fração (o divisor) |
| $-\left(\frac{1}{2} - \frac{1}{3}\right) = -\frac{1}{2} - \frac{1}{3}$ | $-\frac{1}{2} + \frac{1}{3}$ | o menos troca o sinal de todos os termos |
| "Média das frações = fração do total" | depende dos pesos | veja o exercício 🟡 7 |

---

## 💻 Conexão com programação e ML

- Com `double`, `1.0/3 + 1.0/3 + 1.0/3` pode não dar exatamente `1.0`, por causa do arredondamento binário. Frações exatas exigem um tipo como a `Fracao` do extra dos exercícios (ou `BigInteger` no numerador e no denominador).
- **Em ML**, cuidado ao **combinar métricas**: a acurácia de dois lotes juntos **não** é a média das acurácias de cada lote quando os lotes têm tamanhos diferentes. É a soma dos acertos dividida pela soma dos totais (uma *média ponderada*). Isso aparece ao agregar métricas por *batch* ou por classe (*micro* vs *macro average*).
- Dividir por uma fração é multiplicar pelo inverso: uma taxa de aprendizado de $\frac{1}{10}$ aplicada a um gradiente é o mesmo que dividir o gradiente por 10.

---

## 🔗 Conexões
- **Usa:** [[Frações e Equivalência]], [[MMC e MDC]] (o denominador comum), [[Expressões Numéricas]] (a ordem das operações), [[Números Inteiros]] (sinais).
- **É usado em:** [[Números Decimais]], [[Razão, Proporção e Regra de Três]], [[Porcentagem]], [[Potenciação]] (expoente negativo vira fração).
- **Na álgebra:** [[Frações Algébricas]] seguem **exatamente** as mesmas regras, com letras no lugar dos números; e resolver [[Equações do 1º Grau]] com frações começa por "tirar o MMC".
- **Mais adiante:** a soma telescópica do exercício 🔴 1 é a semente das [[Séries Geométricas Infinitas]] e das [[Somas de Riemann]].
- **Treino:** [[Treino Misto de Aritmética]].

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Por que não se pode somar $\frac{1}{2} + \frac{1}{3}$ "direto"? Calcule.
2. Qual é a regra da multiplicação? Por que se pode simplificar "em cruz" antes de multiplicar?
3. Explique, com a ideia de "quantos cabem", por que $2 \div \frac{1}{3} = 6$.
4. Qual é o inverso de $-\frac{3}{8}$? E de $5$? E de $0$?
5. Calcule $\frac{\frac{2}{3}}{\frac{4}{9}}$.
6. Qual é a diferença entre $\left(\frac{2}{3}\right)^2$ e $\frac{2^2}{3}$?
