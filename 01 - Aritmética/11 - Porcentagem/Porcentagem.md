---
tipo: conceito
tema: Aritmética
concluido: false
concluido_em:
proxima_revisao:
conteudo_pronto: true
aliases:
  - Percentual
  - Fator multiplicativo
  - Juros compostos
  - Juros simples
tags:
  - aritmetica
---
# Porcentagem

> [!abstract] Em uma frase
> $p\%$ é só a fração $\frac{p}{100}$. A ferramenta mais poderosa aqui é o **fator multiplicativo**: aumentar $p\%$ é multiplicar por $\left(1 + \frac{p}{100}\right)$, e variações sucessivas se **multiplicam**, nunca se somam.

**Tema:** [[Aritmética]] · **Pré-requisitos:** [[Razão, Proporção e Regra de Três]], [[Números Decimais]] · **Próximo:** [[Potenciação]]
**Praticar:** [[Porcentagem - Exercícios]] · [[Porcentagem - Gabarito]]

## ✅ Etapas
- [ ] Ler a explicação com o caderno aberto e resumir com as minhas palavras
- [ ] Refazer os exemplos resolvidos no caderno, sem olhar
- [ ] Fazer os exercícios 🟢 fáceis e 🟡 médios e corrigir pelo gabarito
- [ ] Anotar os erros no [[Caderno de Erros]]
- [ ] Tentar os 🔴 difíceis
- [ ] Responder à revisão ativa sem consultar
- [ ] Marcar `concluido`, preencher `concluido_em` e `proxima_revisao` (+7 dias)

## 🎯 Ao final, você deve conseguir
- Converter entre porcentagem, fração e decimal, e calcular porcentagens de cabeça.
- Usar o **fator multiplicativo** em aumentos, descontos e variações sucessivas.
- Achar o **valor original** depois de um aumento ou desconto.
- Diferenciar **pontos percentuais** de **porcentagem**.
- Calcular **juros simples** e **compostos**.

---

## 1. O que é porcentagem

$$p\% = \frac{p}{100} \qquad 15\% = \frac{15}{100} = \frac{3}{20} = 0{,}15$$

| % | Fração | Decimal |
|---|---|---|
| 50% | $\frac{1}{2}$ | 0,5 |
| 25% | $\frac{1}{4}$ | 0,25 |
| 20% | $\frac{1}{5}$ | 0,2 |
| 10% | $\frac{1}{10}$ | 0,1 |
| 12,5% | $\frac{1}{8}$ | 0,125 |
| 150% | $\frac{3}{2}$ | 1,5 |

## 2. Os três tipos de pergunta

| Pergunta | Conta | Exemplo |
|---|---|---|
| Quanto é **p% de y**? | $\frac{p}{100} \cdot y$ | 15% de 200 $= 0{,}15 \cdot 200 = 30$ |
| **a** é que % de **b**? | $\frac{a}{b} \cdot 100$ | 18 de 72: $\frac{18}{72} = 0{,}25 = 25\%$ |
| p% de **quanto** dá a? | $a \div \frac{p}{100}$ | 30% de quanto dá 45? $45 \div 0{,}3 = 150$ |

> [!tip] Cálculo mental
> - **10%**: ande a vírgula uma casa para a esquerda (10% de 360 = 36).
> - **5%**: metade de 10% (18). **1%**: duas casas (3,6). **20%**: o dobro de 10% (72).
> - **Troca:** $a\%$ de $b$ = $b\%$ de $a$. Assim, 8% de 50 = 50% de 8 = 4.

## 3. O fator multiplicativo

| Situação | Fator | Exemplo |
|---|---|---|
| **Aumento** de $p\%$ | $1 + \frac{p}{100}$ | +8% → $\times 1{,}08$ |
| **Desconto** de $p\%$ | $1 - \frac{p}{100}$ | −25% → $\times 0{,}75$ |

Um salário de R\$ 2.500 com aumento de 8% vira $2500 \cdot 1{,}08 = 2700$, numa conta só.

> [!important] Variações sucessivas se multiplicam
> +10% e depois −10%:
> $$1{,}10 \cdot 0{,}90 = 0{,}99 \Rightarrow \text{o valor final é } 1\% \text{ menor que o original}$$
> **Não** volta ao valor inicial! O segundo percentual incide sobre uma base **maior**.

**Voltar ao valor original:** se, depois de 20% de desconto, algo custa R\$ 1.200, então $0{,}8 \cdot P = 1200$ e $P = \frac{1200}{0{,}8} = 1500$. (Somar 20% de volta daria 1.440, o que está **errado**.)

## 4. Variação percentual

$$\text{variação} = \frac{\text{novo} - \text{antigo}}{\text{antigo}}$$

Uma ação que vai de R\$ 40 para R\$ 34 tem variação $\frac{34 - 40}{40} = -0{,}15 = -15\%$.

> [!warning] Pontos percentuais × porcentagem
> A acurácia de um modelo subiu de **80% para 88%**:
> - aumentou **8 pontos percentuais** (p.p.), que é a diferença $88 - 80$;
> - aumentou **10%**, que é a variação relativa $\frac{88 - 80}{80}$.
>
> Notícias e relatórios confundem os dois o tempo todo.

## 5. Juros

- **Simples** (o juro incide sempre sobre o capital inicial): $J = C \cdot i \cdot t$, e o montante é $M = C + J$.
- **Compostos** (juros sobre juros; cada período multiplica pelo mesmo fator):
$$M = C \cdot (1 + i)^t$$
R\$ 1.000 a 10% ao ano por 3 anos: $1000 \cdot 1{,}1^3 = 1000 \cdot 1{,}331 = 1331$.

O expoente $t$ é o que faz os juros compostos crescerem tão rápido. É o começo da [[Função Exponencial]] (e uma [[Progressão Geométrica]]).

---

## 📝 Exemplos resolvidos

> [!example] Exemplo 1
> Um produto de R\$ 80 tem 25% de desconto: $80 \cdot 0{,}75 = 60$.

> [!example] Exemplo 2: sucessivos
> Um preço sobe 20% e depois mais 30%. O aumento total é $1{,}2 \cdot 1{,}3 = 1{,}56$, ou seja, **56%** (e não 50%).

> [!example] Exemplo 3: porcentagem de porcentagem
> 40% dos alunos são meninas, e 25% das meninas usam óculos. Que porcentagem do total são meninas de óculos? $0{,}4 \cdot 0{,}25 = 0{,}1 = 10\%$.

> [!example] Exemplo 4: juros simples
> R\$ 2.000 a 1,5% ao mês por 8 meses: $J = 2000 \cdot 0{,}015 \cdot 8 = 240$, e $M = 2240$.

---

## ⚠️ Erros comuns

| ❌ Errado | ✅ Certo | Por quê |
|---|---|---|
| +20% e −20% "se anulam" | $1{,}2 \cdot 0{,}8 = 0{,}96$ → −4% | as bases são diferentes |
| Original de "1200 após −20%" = 1440 | $1200 \div 0{,}8 = 1500$ | divida pelo fator |
| "Subiu de 80% para 88%: subiu 8%" | 8 **p.p.**, ou 10% | |
| +20% e +30% = +50% | $1{,}2 \cdot 1{,}3 = 1{,}56$ → +56% | multiplique os fatores |
| 5% = 0,5 | 5% = 0,05 | $\frac{5}{100}$ |

---

## 💻 Conexão com programação e ML

- Em C#, `0.15.ToString("P")` mostra `15,00 %` (em pt-BR). Guarde porcentagens como **fração** (0,15) no código e formate só na exibição.
- Juros compostos num laço: `for (int i = 0; i < t; i++) m *= 1 + taxa;`, que é o mesmo que `c * Math.Pow(1 + taxa, t)`.
- **Em ML:**
  - O **decaimento da taxa de aprendizado** costuma multiplicar a taxa por um fator a cada época ($\alpha \leftarrow 0{,}9 \cdot \alpha$): é um "desconto composto", ou seja, decaimento exponencial.
  - Relatórios de modelos falam em "ganho de 2 p.p. de acurácia": saiba distinguir de "2%".
  - *Dropout* de 20% desliga, em média, 20% dos neurônios em cada passo de treino.

---

## 🔗 Conexões
- **Usa:** [[Frações e Equivalência]], [[Números Decimais]], [[Razão, Proporção e Regra de Três]] (porcentagem é uma razão com denominador 100).
- **É usado em:** [[Potenciação]] ($1{,}1^3$ nos juros compostos).
- **Na álgebra:** problemas de porcentagem com incógnita viram [[Equações do 1º Grau]].
- **Mais adiante:** [[Função Exponencial]] e [[O Número e]] (juros compostos contínuos), [[Progressão Geométrica]], [[Probabilidade Básica]] (probabilidades em %), [[Tabelas de Frequência e Gráficos]] (frequência relativa).

---

## 🧠 Revisão ativa
*Responda sem olhar. Travou? Releia a seção correspondente.*

1. Como calcular 15% de 80 de cabeça?
2. Qual é o fator multiplicativo de um aumento de 35%? E de um desconto de 35%?
3. Por que +10% seguido de −10% não volta ao valor inicial?
4. Um preço com 15% de desconto ficou em R\$ 170. Qual era o preço original?
5. Qual é a diferença entre "subiu 5 pontos percentuais" e "subiu 5%"?
6. Escreva a fórmula dos juros compostos e explique o papel do expoente.
